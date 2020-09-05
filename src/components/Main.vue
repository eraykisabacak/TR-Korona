<template>
  <div>
    <div class="main-content-wrapper">
      <div class="content-section-1">
        <div class="container">
          <div class="row">
            <div class="row mtn-25 worldwide-stats">
              <div class="col-md-6">
                <div class="tracker-block-style-1">
                  <div class="tracker-block">
                    <div class="tracker-block__icon">
                      <img
                        src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-red.png"
                        alt="corona-icon"
                      />
                    </div>
                    <div class="tracker-block__content">
                      <h4>Toplam Vaka</h4>
                      <h2>
                        <span class="cases-no infected">
                          {{
                          this.allData[0].toplam_vaka
                          }}
                        </span>
                        <span class="new-no">
                          (+
                          <span class="today_infected">{{this.allData[0].gunluk_vaka}}</span>)
                        </span>
                      </h2>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="tracker-block-style-1">
                  <div class="tracker-block">
                    <div class="tracker-block__icon">
                      <img
                        src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-green.png"
                        alt="corona-icon"
                      />
                    </div>
                    <div class="tracker-block__content">
                      <h4>Toplam İyileşen</h4>
                      <h2>
                        <span class="cases-no infected">
                          {{
                          this.allData[0].toplam_iyilesen
                          }}
                        </span>
                        <span class="new-no">
                          (+
                          <span class="today_infected">{{this.allData[0].gunluk_iyilesen}}</span>)
                        </span>
                      </h2>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="tracker-block-style-1">
                  <div class="tracker-block">
                    <div class="tracker-block__icon">
                      <img
                        src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-red.png"
                        alt="corona-icon"
                      />
                    </div>
                    <div class="tracker-block__content">
                      <h4>Toplam Vefat</h4>
                      <h2>
                        <span class="cases-no infected">{{this.allData[0].toplam_vefat}}</span>
                        <span class="new-no">
                          (+
                          <span class="today_infected">{{this.allData[0].gunluk_vefat}}</span>)
                        </span>
                      </h2>
                    </div>
                  </div>
                </div>
              </div>
              <div class="col-md-6">
                <div class="tracker-block-style-1">
                  <div class="tracker-block">
                    <div class="tracker-block__icon">
                      <img
                        src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-red.png"
                        alt="corona-icon"
                      />
                    </div>
                    <div class="tracker-block__content">
                      <h4>Ağır Hasta</h4>
                      <h2>
                        <span class="cases-no infected">{{this.allData[0].agir_hasta_sayisi}}</span>
                        <span class="new-no">
                          (+
                          <span class="today_infected">{{this.getAgir()}}</span>)
                        </span>
                      </h2>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

let config = {
  headers: {
    Accept: "application/json, text/plain, */*",
  },
};

export default {
  data() {
    return {
      allData: {},
    };
  },
  methods: {
    getAgir() {
      let todayAgirHasta = this.allData[0].agir_hasta_sayisi.replace(".", "");
      let yesterdayAgirHasta = this.allData[1].agir_hasta_sayisi.replace(
        ".",
        ""
      );

      return todayAgirHasta - yesterdayAgirHasta;
    },
  },
  created() {
    axios
      .get("https://covid19.saglik.gov.tr/covid19api?getir=liste", config)
      .then(
        (response) => {
          this.allData = response.data;
          console.log(this.allData);
        },
        (error) => {
          console.log(error);
        }
      );
  },
};
</script>

<style scoped>
.main-content-wrapper {
  background-color: #f7f8fc;
  padding: 90px 0;
}
.tracker-block__icon {
  -webkit-flex-basis: 57px;
  -ms-flex-preferred-size: 57px;
  flex-basis: 57px;
  width: 57px;
  margin-right: 20px;
}
.row {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap;
  flex-wrap: wrap;
  margin-right: -15px;
  margin-left: -15px;
}
.mtn-25 {
  margin-top: -25px;
}
.tracker-block {
  background-color: #ffffff;
  display: -webkit-box;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -webkit-align-items: center;
  -ms-flex-align: center;
  align-items: center;
  margin-top: 25px;
  padding: 25px 0 25px 30px;
}
.tracker-block__icon {
  -webkit-flex-basis: 57px;
  -ms-flex-preferred-size: 57px;
  flex-basis: 57px;
  width: 57px;
  margin-right: 20px;
}
div {
  display: block;
}
.tracker-block__content h2 {
  color: #222222;
  font-size: 30px;
  font-weight: 700;
  margin-bottom: 0;
}
.tracker-block__content h4 {
  color: #4d4d4d;
  font-size: 18px;
  font-weight: 400;
}
.tracker-block__content h2 .new-no {
  color: #4d4d4d;
  font-size: 18px;
  font-weight: 400;
  vertical-align: middle;
}
</style>

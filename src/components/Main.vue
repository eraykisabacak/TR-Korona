<template>
  <div>
    <div class="main-content-wrapper">
      <h1
        style="display: flex;flex-direction: column;justify-content: center;text-align: center;"
      >{{this.allData[0].tarih}} - Günlük Rapor</h1>
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
                      <h4>Bugünkü Test Sayısı</h4>
                      <h2>
                        <span class="cases-no infected">
                          {{
                          this.allData[0].gunluk_test
                          }}
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
                      <h4>Bugünkü Hasta Sayısı</h4>
                      <h2>
                        <span class="cases-no infected">
                          {{
                          this.allData[0].gunluk_vaka
                          }}
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
                      <h4>Bugünkü Vefat Sayısı</h4>
                      <h2>
                        <span class="cases-no infected">{{this.allData[0].gunluk_vefat}}</span>
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
                      <h4>Bugünkü İyileşen Sayısı</h4>
                      <h2>
                        <span class="cases-no infected">{{this.allData[0].gunluk_iyilesen}}</span>
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
    <div class="main-content-wrapper">
      <h1
        style="display: flex;flex-direction: column;justify-content: center;text-align: center;"
      >Tüm Zamanların Raporu</h1>
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
            <div class="col-lg-12 mt-5">
              <div class="list-view table-responsive" id="list-view">
                <div id="DataTables_Table_0_wrapper" class="dataTables_wrapper no-footer">
                  <div class="dataTables_length" id="DataTables_Table_0_length"></div>
                  <div id="DataTables_Table_0_filter" class="dataTables_filter"></div>
                  <table
                    class="list-view__table display table dataTable no-footer"
                    id="DataTables_Table_0"
                    role="grid"
                    aria-describedby="DataTables_Table_0_info"
                  >
                    <thead class="list-view__head">
                      <tr role="row">
                        <th
                          class="sorting_asc"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-sort="ascending"
                          aria-label="Region: activate to sort column descending"
                          style="width: 281px;"
                        >Gün</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="Total Cases: activate to sort column ascending"
                          style="width: 84px;"
                        >Toplam Vaka</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="New Cases: activate to sort column ascending"
                          style="width: 80px;"
                        >Bugünkü Vaka</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="Total Deaths: activate to sort column ascending"
                          style="width: 90px;"
                        >Toplam Vefat</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="Deaths %: activate to sort column ascending"
                          style="width: 67px;"
                        >Deaths %</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="New Deaths: activate to sort column ascending"
                          style="width: 86px;"
                        >Bugünkü Vefat</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="Total Recovered: activate to sort column ascending"
                          style="width: 117px;"
                        >Toplam İyileşen</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="Total Recovered: activate to sort column ascending"
                          style="width: 117px;"
                        >Bugünkü İyileşen</th>
                        <th
                          class="sorting"
                          tabindex="0"
                          aria-controls="DataTables_Table_0"
                          rowspan="1"
                          colspan="1"
                          aria-label="Recovered %: activate to sort column ascending"
                          style="width: 92px;"
                        >Recovered %</th>
                      </tr>
                    </thead>

                    <tbody class="list-view__body">
                      <tr
                        class="country-item odd"
                        role="row"
                        v-for="item in allData"
                        :key="item.tarih"
                      >
                        <td class="sorting_1">{{item.tarih}}</td>
                        <td>{{item.toplam_vaka}}</td>
                        <td>{{item.gunluk_vaka}}</td>
                        <td>{{item.toplam_vefat}}</td>
                        <td>{{(parseInt(item.toplam_vefat) / parseInt(item.toplam_vaka) * 100).toFixed(2)}}%</td>
                        <td>{{item.gunluk_vefat}}</td>
                        <td>{{item.toplam_iyilesen}}</td>
                        <td>{{item.gunluk_iyilesen}}</td>
                        <td>{{(parseInt(item.toplam_iyilesen) / parseInt(item.toplam_vaka) * 100).toFixed(2)}}%</td>
                      </tr>
                    </tbody>
                  </table>
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
      .get(
        "https://koronacors.herokuapp.com/?https://covid19.saglik.gov.tr/covid19api?getir=liste",
        config
      )
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
  /*
  <div class="row mtn-25 worldwide-stats" style="margin-top: 25px;">
              
            </div>*/
};
</script>

<style scoped>
.main-content-wrapper {
  background-color: #f7f8fc;
  padding: 25px 0;
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
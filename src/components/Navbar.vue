<template>
  <header class="header-wrapper">
    <div class="container">
      <div class="row justify-content-between align-items-center">
        <div class="col-lg-4">
          <div class="logo-wrap">
            <a href="index.html" style="text-decoration: none;">
              <img
                src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-green.png"
                alt="logo"
              />
              <img
                src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-green.png"
                alt="logo"
              />
              <img
                src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/corona-icon-green.png"
                alt="logo"
              />
            </a>
          </div>
        </div>

        <div class="col-md-6 col-lg-4">
          <div class="last-update-wrap">
            <p class="mb-0">
              Bilgiler:
              <span
                class="last-update"
              >Türkiye Cumhuriyeti Sağlık Bakanlığınden Alınmaktadır</span>
            </p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4">
          <div class="navbar-wrap">
            <nav class="menubar">
              <ul class="nav">
                <li>
                  <a
                    href="https://github.com/eraykisabacak/TR-Korona"
                    style="margin-right:35px"
                  >Github</a>
                </li>
                <li>
                  <a
                    href="https://www.linkedin.com/in/eraykisabacak/"
                    style="margin-right:35px"
                  >Linkedin</a>
                </li>
                <li>
                  <a href="https://eraykisabacak.com/" style="margin-right:35px">Website</a>
                </li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style scoped>
.header-wrapper {
  padding: 20px 0;
}
.last-update-wrap {
  color: #4d4d4d;
  font-size: 14px;
  font-style: italic;
  font-weight: 300;
  text-align: center;
}
.menubar .nav li a {
  font-weight: 500;
  color: #171717;
}
a {
  -webkit-transition: 0.4s;
  -o-transition: 0.4s;
  transition: 0.4s;
  outline: none;
  text-decoration: none;
}
ul {
  margin: 0;
  padding: 0;
}
.nav {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap;
  flex-wrap: wrap;
  padding-left: 0;
  margin-bottom: 0;
  list-style: none;
}
.menubar .nav {
  -webkit-box-pack: end;
  -webkit-justify-content: flex-end;
  -ms-flex-pack: end;
  justify-content: flex-end;
}
</style>

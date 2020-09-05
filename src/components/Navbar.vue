<template>
  <header class="header-wrapper">
    <div class="container">
      <div class="row justify-content-between align-items-center">
        <div class="col-lg-4">
          <div class="logo-wrap">
            <a href="index.html"
              ><img
                src="https://live.hasthemes.com/html/8/jibanu-preview/jibanu/assets/img/logo.png"
                alt="logo"
            /></a>
          </div>
        </div>

        <div class="col-md-6 col-lg-4">
          <div class="last-update-wrap">
            <p class="mb-0">
              Update: <span class="last-update">05.09.2020 at 21:47:23</span>
            </p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4">
          <div class="navbar-wrap">
            <nav class="menubar">
              <ul class="nav">
                <li>
                  <a href="index.html" style="margin-right:35px">Dashboard</a>
                </li>
                <li><a href="map.html" style="margin-right:35px">Map</a></li>
                <li>
                  <a href="badge.html" style="margin-right:35px">Badge</a>
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

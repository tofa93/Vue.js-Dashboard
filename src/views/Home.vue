<template>
  <div class="content">
    <div class="dashboard">
      <div class="dash-block"></div>
      <div class="dash-block"></div>
      <div class="dash-block"></div>
      <div class="dash-block"></div>
      <div class="dash-block"></div>
    </div>
    <div class="section-intro">Entertainment</div>
    <div class="content-main">
      <div class="ent-block">
        <router-link to="/music">
          <img src="../assets/banners/music-banner.jpg" alt="" class="banner-img">
        </router-link>
      </div>
      <div class="ent-block">
        <router-link to="/books">
          <img src="../assets/banners/books-banner.jpg" alt="" class="banner-img">
        </router-link>
      </div>
      <div class="ent-block">
        <router-link to="/movies">
          <img src="../assets/banners/movies-banner.jpeg" alt="" class="banner-img">
        </router-link>
      </div>
      <div class="ent-block">
        <router-link to="/animes">
          <img src="../assets/banners/animes-banner.jpg" alt="" class="banner-img">
        </router-link>
      </div>
    </div>
    <div class="section-intro">Business</div>
    <div class="content-main">
      <div class="bsn-block" id="eCommerce">
        <router-link to="/commerce">
          <img src="../assets/banners/e_commerce-banner.jpg" alt="" class="banner-img">
        </router-link>
      </div>
      <div class="bsn-block">
        <router-link to="/weather">
          <img src="../assets/banners/weather-banner.png" alt="" class="banner-img">
        </router-link>
      </div>
      <div class="bsn-block">
        <router-link to="/notes">
          <img src="../assets/banners/notes-banner.jpg" alt="" class="banner-img">
        </router-link>
      </div>
      <div class="bsn-block" id="workSter">
        <router-link to="/work">
          <img src="../assets/banners/work-banner.jpg" alt="" class="banner-img">
        </router-link>
      </div>
    </div>
    <div class="section-intro">Future projects</div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {}
}
</script>

<style>
.dashboard {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
  width: 100%;
  font-size: 28px;
  font-weight: 700;
  letter-spacing: .7mm;
}

.dash-block {
  padding: 1rem;
  height: 275px;
  border: 1px solid #343434;
}

.dash-block:nth-child(5) {
  grid-column: 2/4;
}

.section-intro {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1rem;
  height: 150px;
  width: 100%;
  font-size: 24px;
  font-weight: 700;
  background-color: #191919;
}

.welcome-title {
  font-size: 36px;
  font-weight: 700;
}

.content-main {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  justify-items: center;
  gap: 10px;
}

.ent-block {
  height: 300px;
  width: 100%;
}

.bsn-block {
  height: 300px;
  width: 100%;
  border: 1px solid #343434;
}

#eCommerce {
  grid-column: 1/4;
}

#workSter {
  grid-column: 2/5;
}

.banner-img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}
</style>

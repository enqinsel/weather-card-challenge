<script setup>
import SliderComp from "./components/SliderComp.vue";
</script>

<template>
  <div class="mask"></div>
  <div class="container">
    <div class="title">
      <span>28 EKİM CUMA</span>
    </div>
    <div class="degreeAndWeather">
      <p>24<sup>&degC</sup></p>

      <div class="degreeAndWeather__img">
        <img src="./assets/partlyCloudy.png" alt="" />
        <span>Parçalı Bulutlu</span>
      </div>
    </div>
    <div class="weatherFeautures">
      <div class="wet">
        <img src="./assets/wet.png" />
        <span>80%</span>
      </div>
      <div class="aqi">
        <img src="./assets/aqi.png" alt="" />
        <span>AQI <span>20</span></span>
      </div>
      <div class="wind">
        <img src="./assets/wind.png" alt="" />
        <span>10 km/s</span>
      </div>
    </div>
    <div class="slider">
      <SliderComp></SliderComp>
    </div>
    <div class="footer">
      <ul class="days">
        <li>CTS</li>
        <li>PZR</li>
        <li>PZT</li>
        <li>SALI</li>
        <li>ÇRŞ</li>
      </ul>
      <ul class="degree">
        <li>24&deg;</li>
        <li>24&deg;</li>
        <li>24&deg;</li>
        <li>24&deg;</li>
        <li>24&deg;</li>
      </ul>
      <ul class="img">
        <li><img src="./assets/partlyCloudy.png" /></li>
        <li><img src="./assets/partlyCloudy.png" /></li>
        <li><img src="./assets/partlyCloudy.png" /></li>
        <li><img src="./assets/partlyCloudy.png" /></li>
        <li><img src="./assets/partlyCloudy.png" /></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.mask {
  width: 200px;
  height: 200px;
  border-radius: 200px;
  position: absolute;
  top: 100px;
  left: 550px;
  background-color: rgb(243, 243, 60);
}
.container {
  width: 500px;
  height: 600px;
  padding: 20px;
  background: rgb(63, 94, 114, 0.25);
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(100px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgb(37, 213, 140,0.2);
  position: relative;
  
}

img {
  width: 80px;
}
.title {
  font-size: 22px;
  color: white;
}

.degreeAndWeather {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
}

.degreeAndWeather p {
  font-size: 82px;
  position: relative;
  color: white;
}

.degreeAndWeather p sup {
  font-size: 32px;
  color: white;
}

.degreeAndWeather__img {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.degreeAndWeather__img span {
  font-size: 22px;
  color: white;
}

.weatherFeautures {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  color: white;
  position: absolute;
  top: 170px;
  left: 0;
  right: 0;
}
.weatherFeautures img {
  width: 20px;
  filter: brightness(0) invert(1);
}

.wet {
  display: flex;
  gap: 10px;
}

.aqi {
  display: flex;
  gap: 10px;
}

.wind {
  display: flex;
  gap: 10px;
}

.slider{
  position: absolute;
  top: 220px;
  left: 40px;
  right: 0;
}

.footer {
  display: flex;
  flex-direction: column;
  color: white;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 55px;
}

.footer .days {
  display: flex;
  justify-content: space-evenly;
}

.footer .degree {
  display: flex;
  justify-content: space-evenly;
}

.footer .img {
  display: flex;
  justify-content: space-evenly;
}

.footer .img img {
  width: 50px;
}
</style>

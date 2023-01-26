<script setup></script>

<template>
  <div class="wrapper">
    <div class="header">
      <img src="../assets/sunrise.png" />
      <input type="range" class="range" value="0" />
      <img src="../assets/sunset.png" />
    </div>
    <div class="section">
      <ul class="exp">
        <li>Hissedilen Sıcaklık</li>
        <li>Nem Durumu</li>
        <li>Yağmur Durumu</li>
        <li>Rüzgar Hızı</li>
      </ul>
      <ul class="numbers">
        <li>25.7&deg;</li>
        <li>80%</li>
        <li>60%</li>
        <li>10km/s</li>
      </ul>
    </div>
  </div>
</template>

<style scope>
.wrapper {
  width: 450px;
  height: 200px;
  padding: 5px;
  background: rgba(255, 255, 255, 0.15);
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(2px);
  -webkit-backdrop-filter: blur(4px);
  border-radius: 10px;
  border: 1px solid rgb(37, 213, 140,0.2);
  position: relative;
}

.header {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
}

.header img {
  width: 100px;
}

.section {
  display: flex;
  flex-direction: column;
  color: white;
  position: absolute;
  bottom: 0;
  left: 0;
  right: 50px;
}

.section .exp {
  display: flex;
  justify-content: space-evenly;
  gap: 50px;
  font-size: 14px;
  opacity: 0.7;
}

.section .exp li {
  margin-left: 5px;
}

.section .numbers {
  display: flex;
  justify-content: space-evenly;
  gap: 50px;
  font-size: 14px;
}

.section .numbers li {
  margin-left: 25px;
}

.range {
  width: 250px;
  height: 15px;
  -webkit-appearance: none;
  background: rgba(255, 255, 255, 0.35);;;
  outline: none;
  border-radius: 15px;
  overflow: hidden;
  margin-top: 10px;
}

.range::-webkit-slider-thumb {
  -webkit-appearance: none;
  width: 15px;
  height: 15px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.15);;
  cursor: pointer;
  border: 4px solid rgb(51, 51, 51);
  box-shadow: -407px 0 0 400px #7999A3;
}
</style>

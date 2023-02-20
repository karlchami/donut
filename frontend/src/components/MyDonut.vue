<template>
  <div class="donut-container">
    <div class="title">give me my <strong>fuck</strong>ing donut.</div>
    <div class="leftEye"></div>
    <div class="rightEye"></div>
    <div class="leftPupil"></div>
    <div class="rightPupil"></div>
    <div class="beard"></div>
    <div class="mouth"></div>
    <div class="nose"></div>
    <div class="x"></div>
    <div class="wrinkle"></div>
    <div id="yummyDonut">
      <div class="donut"></div>
      <div class="inner"></div>
    </div>
  </div>
</template>

<style>
*{
  margin: 0;
  padding: 0;
}
body{
  background: #FED90F;
}
div{
  position: absolute;
}
.title{
  white-space: nowrap;
  left: 78px;
}
.nose{
  width: 45px;
  height: 38px;
  top: 135px;
  left: 140px;
  border-radius: 50%;
  background: #FED90F;
  border: solid 4px black;
  box-shadow:1px 8px 10px #202020, inset -4px -3px  rgb(197, 147, 39);
}
.leftEye{
  width: 70px;
  height: 70px;
  top: 80px;
  left: 85px;
  border-radius: 50%;
  background: white;
  border: solid 5px rgb(24, 24, 24);
}
.rightEye{
  width: 70px;
  height: 70px;
  top: 80px;
  left: 170px;
  border-radius: 50%;
  background: white;
  border: solid 5px black;
}
.leftPupil{
  width: 10px;
  height: 10px;
  top: 120px;
  left: 120px;
  border-radius: 50%;
  background: black;
  animation: leftEyeMovement 3s linear 0s infinite;
  animation-direction: alternate;
}
.rightPupil{
  width: 10px;
  height: 10px;
  top: 120px;
  left: 205px;
  border-radius: 50%;
  background: black;
  animation: rightEyeMovement 3s linear 0s infinite;
  animation-direction: alternate;
}
.beard{
  width: 160px;
  height: 130px;
  top: 155px;
  left: 85px;
  border-radius: 50%;
  background: #d1af74;
  border: solid 5px black;
  box-shadow: inset -4px -3px  rgb(150, 110, 24);
}
.mouth{
  background:#d1af74;;
  width: 140px;
  height: 80px;
  top: 170px;
  left: 95px;
  border-radius: 50%;
  border: solid 4px #d1af74;;
  border-bottom-color: black;
}
.x{
  width: 10px;
  height: 10px;
  top: 135px;
  left: 162.5px;
  background: #FED90F;
}
.wrinkle{
  width: 30px;
  height: 10px;
  top: 260px;
  left: 150px;
  background: #d1af74;;
  border-radius: 50%;
  border: solid 2px #d1af74;
  border-bottom-color: black;
}
.donut{
  width: 90px;
  height: 90px;
  top: 260px;
  left: 20px;
  border-radius: 50%;
  background-color:rgb(248, 10, 129);
  background-image: radial-gradient(white 10%, transparent 11%), radial-gradient(white 10%, transparent 11%);
  background-size: 30px 30px;
  background-position: 0 0, 30px 30px;
  border: solid black 4px;
  box-shadow: inset -3px -2px rgb(216, 122, 0), 1px 8px 10px #202020;
}
.inner{
  width: 30px;
  height: 30px;
  top: 290px;
  left: 50px;
  border-radius: 50%;
  background: #FED90F;
  border: solid black 3px;
  box-shadow:  inset 1px 4px 6px #202020, 0px 0px 5px 6px white;
}

#yummyDonut{
  animation: donutMovement 3s linear 0s infinite;
  animation-direction: alternate;
}

@keyframes leftEyeMovement {
  from{left:105px;}
  to{left:130px;}
}

@keyframes rightEyeMovement {
  from{left:190px;}
  to{left:215px;}
}
@keyframes donutMovement {
  from{left:25px;}
  to{left:215px;}
}
</style>

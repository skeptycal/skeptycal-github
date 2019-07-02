<template>
  <div class="VueToNuxtLogo">
    <div class="Triangle Triangle--two" />
    <div class="Triangle Triangle--one" />
    <div class="Triangle Triangle--three" />
    <div class="Triangle Triangle--four" />
  </div>
</template>

<style>
.VueToNuxtLogo {
  display: flex;
  float: inline-start;
  animation: turn 2s linear forwards 1s;
  transform: rotateX(180deg);
  position: relative;
  overflow: hidden;
  height: 80%;
  padding: 3px;
  /*  height: 180px;
  width: 245px; */
}

.Triangle {
  /* animation: shrink 0.5s linear forwards 3.5s; */
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 0;
}

.Triangle--one {
  /* animation: shrink 0.5s linear forwards 3.5s; */
  border-left: 52px solid transparent;
  border-right: 52px solid transparent;
  border-bottom: 90px solid #41b883;
}

.Triangle--two {
  top: 15px;
  left: 17px;
  animation: goright 0.5s linear forwards 3.5s;
  /* animation: shrink 0.5s linear forwards 3.5s; */

  border-left: 44px solid transparent;
  border-right: 44px solid transparent;
  border-bottom: 75px solid #3b8070;
}

.Triangle--three {
  top: 30px;
  left: 17px;
  animation: goright 0.5s linear forwards 3.5s;
  /* animation: shrink 0.5s linear forwards 3.5s; */

  border-left: 35px solid transparent;
  border-right: 35px solid transparent;
  border-bottom: 60px solid #35495e;
}

.Triangle--four {
  top: 60px;
  left: 35px;
  animation: godown 0.5s linear forwards 3s;
  /* animation: shrink 0.5s linear forwards 3.5s; */

  border-left: 17px solid transparent;
  border-right: 17px solid transparent;
  border-bottom: 30px solid #fff;
}

@keyframes shrink {
  100% {
    transform: translate3d(0.3);
    transform: scale(0.3);
  }
}

@keyframes turn {
  100% {
    transform: rotateX(0deg);
  }
}

@keyframes godown {
  100% {
    top: 180px;
  }
}

@keyframes goright {
  100% {
    left: 35px;
  }
}
</style>


<style>
  body {
    background-color: #292030;
  }

  /* GRADIENT CIRCLE */
  .gradient {
    z-index: -2;
    box-shadow: inset 0px 0px 65px 32px rgba(0, 0, 0, 0.75);
    width: 90vh;
    height: 90vh;
    position: relative;
    border-radius: 50%;
    margin-top: 5vh;
    margin-left: auto;
    margin-right: auto;
    overflow: hidden;
  }
  .gradient h2 {
    text-align: center;
    color: white;
    font-family: "Lobster";
    font-size: 45px;
    padding-top: 60vh;
  }

  /* CHIMES */
  .chime {
    position: absolute;
    left: 150px;
    top: 0;
    height: 250px;
    width: 64px;
    animation-name: rotate;
    animation-duration: 2s;
    animation-delay: 0.7s;
    animation-iteration-count: infinite;
    animation-direction: linear;
    transform-origin: 50% 0%;
    animation-timing-function: linear;
  }
  .chime:before {
    content: "";
    background-color: #726c76;
    position: absolute;
    height: 100%;
    width: 1px;
    left: calc(50% - 1px);
    top: 0;
    border-right: 1px solid #5d5960;
  }

  .ball {
    width: 64px;
    height: 64px;
    background-color: #a12d1f;
    border-radius: 50%;
    position: absolute;
    bottom: 0;
    left: 0;
  }
  .ball:after {
    position: absolute;
    content: " ";
    width: 85.9375%;
    height: 85.9375%;
    background-color: #f34f4d;
    z-index: 1;
    border-radius: 50%;
    top: 1px;
    left: 2px;
  }

  .small-ball {
    position: absolute;
    width: 23.4375%;
    height: 23.4375%;
    background: #fff;
    top: 31.25%;
    left: 23.4375%;
    z-index: 2;
    border-radius: 50%;
  }

  .tiny {
    width: 10.9375%;
    height: 10.9375%;
    top: 15.625%;
    left: 46.875%;
  }

  .red.red2 {
    left: 550px;
    height: 180px;
    width: 70px;
    animation-name: rotate5;
    animation-duration: 2.5s;
    animation-delay: 0.3s;
    animation-iteration-count: infinite;
    animation-direction: linear;
    transform-origin: 50% 0%;
    animation-timing-function: linear;
  }
  .red.red2 .ball {
    width: 70px;
    height: 70px;
  }

  .orange {
    left: 300px;
    height: 200px;
    width: 32px;
    animation-name: rotate5;
    animation-duration: 3s;
    animation-delay: 0.1s;
    animation-iteration-count: infinite;
    animation-direction: linear;
    transform-origin: 50% 0%;
    animation-timing-function: linear;
  }
  .orange .ball {
    width: 32px;
    background-color: #e28124;
    height: 32px;
  }
  .orange .ball:after {
    background-color: #fdb868;
  }
  .orange.orange2 {
    left: 700px;
    height: 280px;
    width: 50px;
    animation-name: rotate;
    animation-duration: 1.5s;
    animation-delay: 0.7s;
    animation-iteration-count: infinite;
    animation-direction: linear;
    transform-origin: 50% 0%;
    animation-timing-function: linear;
  }
  .orange.orange2 .ball {
    width: 50px;
    height: 50px;
  }

  .blue {
    left: 450px;
    height: 270px;
    width: 50px;
    animation-name: rotate10;
    animation-duration: 1.5s;
    animation-delay: 0.5s;
    animation-iteration-count: infinite;
    animation-direction: linear;
    transform-origin: 50% 0%;
    animation-timing-function: linear;
  }
  .blue .ball {
    width: 50px;
    background-color: #2261a3;
    height: 50px;
  }
  .blue .ball:after {
    background-color: #3abbda;
  }

  /* MOONS */
  .moon {
    position: absolute;
    width: 15px;
    height: 15px;
    background-color: #f5e849;
    border-radius: 50%;
    animation: glow 3.5s linear infinite alternate;
  }
  .moon:before {
    content: " ";
    width: 50px;
    height: 50px;
    background: radial-gradient(ellipse at center, rgba(255, 255, 255, 0.3) 0%, rgba(255, 255, 255, 0.1) 35%, rgba(255, 255, 255, 0) 45%, rgba(255, 255, 255, 0) 100%);
    z-index: -1;
    border-radius: 50%;
    top: calc(50% - 25px);
    left: calc(50% - 25px);
    position: absolute;
  }
  .moon.m1 {
    top: 20%;
    left: 10%;
    width: 20px;
    height: 20px;
  }
  .moon.m2 {
    top: 40%;
    left: 15%;
    width: 15px;
    height: 15px;
  }
  .moon.m3 {
    top: 5%;
    left: 45%;
    width: 25px;
    height: 25px;
    background-color: #4af1c6;
    animation: glowblue 1.5s linear infinite alternate;
  }
  .moon.m3:before {
    content: " ";
    width: 80px;
    height: 80px;
    background: radial-gradient(ellipse at center, rgba(255, 255, 255, 0.3) 0%, rgba(255, 255, 255, 0.1) 35%, rgba(255, 255, 255, 0) 45%, rgba(255, 255, 255, 0) 100%);
    z-index: -1;
    border-radius: 50%;
    top: calc(50% - 40px);
    left: calc(50% - 40px);
    position: absolute;
  }
  .moon.m4 {
    top: 55%;
    left: 45%;
  }
  .moon.m5 {
    top: 50%;
    left: 25%;
  }
  .moon.m6 {
    top: 10%;
    left: 75%;
  }
  .moon.m7 {
    top: 50%;
    left: 55%;
    background-color: #e74c3c;
    animation: glowred 1.5s linear infinite alternate;
    width: 10px;
    height: 10px;
  }
  .moon.m8 {
    top: 60%;
    left: 70%;
  }
  .moon.m9 {
    top: 35%;
    left: 80%;
    width: 10px;
    height: 10px;
  }
  .moon.m10 {
    top: 80%;
    left: 15%;
    width: 20px;
    height: 20px;
  }

  /* STARS */
  .star {
    position: absolute;
    width: 15px;
    height: 15px;
    background: transparent;
  }
  .star:before {
    content: " ";
    height: 25%;
    width: 100%;
    top: 50%;
    transform: translateY(-50%);
    position: absolute;
    background: #f5f5f5;
    border-radius: 50%;
    animation: glowstar 3.5s linear infinite alternate;
  }
  .star:after {
    content: " ";
    height: 100%;
    width: 25%;
    left: 50%;
    transform: translateX(-50%);
    position: absolute;
    background: #f5f5f5;
    border-radius: 50%;
    animation: glowstar 3.5s linear infinite alternate;
  }
  .star.s1 {
    top: 24%;
    left: 45%;
    filter: blur(0.3px);
  }
  .star.s2 {
    top: 43%;
    left: 35%;
    width: 15px;
    height: 15px;
    filter: blur(1.5px);
  }
  .star.s3 {
    top: 15%;
    left: 21%;
    width: 25px;
    height: 25px;
    filter: blur(1.5px);
  }
  .star.s4 {
    top: 22%;
    left: 33%;
    filter: blur(0.1px);
  }
  .star.s5 {
    top: 44%;
    left: 55%;
    filter: blur(0.8px);
  }
  .star.s6 {
    top: 66%;
    left: 77%;
    filter: blur(0.7px);
  }
  .star.s7 {
    top: 12%;
    left: 67%;
    width: 10px;
    height: 10px;
    filter: blur(0.6px);
  }
  .star.s8 {
    top: 29%;
    left: 78%;
    filter: blur(1.2px);
  }
  .star.s9 {
    top: 15%;
    left: 81%;
    width: 10px;
    height: 10px;
    filter: blur(1.8px);
  }
  .star.s10 {
    top: 30%;
    left: 65%;
    width: 20px;
    height: 20px;
    filter: blur(0.2px);
  }

  /* ROTATE ANIMATION */
  @-webkit-keyframes rotate {
    0% {
      transform: rotate(-15deg);
      animation-timing-function: ease-in;
    }
    25% {
      transform: rotate(0deg);
      animation-timing-function: ease-out;
    }
    50% {
      transform: rotate(15deg);
      animation-timing-function: ease-in;
    }
    75% {
      transform: rotate(0deg);
      animation-timing-function: ease-out;
    }
    100% {
      transform: rotate(-15deg);
    }
  }
  @-webkit-keyframes rotate10 {
    0% {
      transform: rotate(-10deg);
      animation-timing-function: ease-in;
    }
    25% {
      transform: rotate(0deg);
      animation-timing-function: ease-out;
    }
    50% {
      transform: rotate(10deg);
      animation-timing-function: ease-in;
    }
    75% {
      transform: rotate(0deg);
      animation-timing-function: ease-out;
    }
    100% {
      transform: rotate(-10deg);
    }
  }
  @-webkit-keyframes rotate5 {
    0% {
      transform: rotate(-5deg);
      animation-timing-function: ease-in;
    }
    25% {
      transform: rotate(0deg);
      animation-timing-function: ease-out;
    }
    50% {
      transform: rotate(5deg);
      animation-timing-function: ease-in;
    }
    75% {
      transform: rotate(0deg);
      animation-timing-function: ease-out;
    }
    100% {
      transform: rotate(-5deg);
    }
  }
  /* GLOW ANIMATION */
  @-webkit-keyframes glow {
    from {
      box-shadow: 0 0 2px rgba(245, 232, 73, 0.7), 0 0 4px rgba(245, 232, 73, 0.7), 0 0 8px rgba(245, 232, 73, 0.7), 0 0 6px rgba(245, 232, 73, 0.3), 0 0 16px rgba(245, 232, 73, 0.3), 0 0 20px rgba(245, 232, 73, 0.3), 0 0 24px rgba(245, 232, 73, 0.3);
    }
    to {
      box-shadow: 0 0 0px rgba(245, 232, 73, 0.7), 0 0 1px rgba(245, 232, 73, 0.7), 0 0 2px rgba(245, 232, 73, 0.7), 0 0 3px rgba(245, 232, 73, 0.3), 0 0 4px rgba(245, 232, 73, 0.3), 0 0 5px rgba(245, 232, 73, 0.3), 0 0 6px rgba(245, 232, 73, 0.3);
    }
  }
  @-webkit-keyframes glowblue {
    from {
      box-shadow: 0 0 2px rgba(93, 242, 205, 0.7), 0 0 4px rgba(93, 242, 205, 0.7), 0 0 8px rgba(93, 242, 205, 0.7), 0 0 6px rgba(93, 242, 205, 0.3), 0 0 16px rgba(93, 242, 205, 0.3), 0 0 20px rgba(93, 242, 205, 0.3), 0 0 24px rgba(93, 242, 205, 0.3);
    }
    to {
      box-shadow: 0 0 0px rgba(93, 242, 205, 0.7), 0 0 1px rgba(93, 242, 205, 0.7), 0 0 2px rgba(93, 242, 205, 0.7), 0 0 3px rgba(93, 242, 205, 0.3), 0 0 4px rgba(93, 242, 205, 0.3), 0 0 5px rgba(93, 242, 205, 0.3), 0 0 6px rgba(93, 242, 205, 0.3);
    }
  }
  @-webkit-keyframes glowred {
    from {
      box-shadow: 0 0 2px rgba(243, 79, 77, 0.7), 0 0 4px rgba(243, 79, 77, 0.7), 0 0 8px rgba(243, 79, 77, 0.7), 0 0 6px rgba(243, 79, 77, 0.3), 0 0 16px rgba(243, 79, 77, 0.3), 0 0 20px rgba(243, 79, 77, 0.3), 0 0 24px rgba(243, 79, 77, 0.3);
    }
    to {
      box-shadow: 0 0 0px rgba(243, 79, 77, 0.7), 0 0 1px rgba(243, 79, 77, 0.7), 0 0 2px rgba(243, 79, 77, 0.7), 0 0 3px rgba(243, 79, 77, 0.3), 0 0 4px rgba(243, 79, 77, 0.3), 0 0 5px rgba(243, 79, 77, 0.3), 0 0 6px rgba(243, 79, 77, 0.3);
    }
  }
  @-webkit-keyframes glowstar {
    from {
      box-shadow: 0 0 2px rgba(245, 232, 73, 0.7), 0 0 4px rgba(245, 232, 73, 0.7), 0 0 8px rgba(245, 232, 73, 0.7), 0 0 6px rgba(245, 232, 73, 0.3), 0 0 16px rgba(245, 232, 73, 0.3), 0 0 20px rgba(245, 232, 73, 0.3), 0 0 24px rgba(245, 232, 73, 0.3);
    }
    to {
      box-shadow: 0 0 0px rgba(245, 232, 73, 0.7), 0 0 1px rgba(245, 232, 73, 0.7), 0 0 2px rgba(245, 232, 73, 0.7), 0 0 3px rgba(245, 232, 73, 0.3), 0 0 4px rgba(245, 232, 73, 0.3), 0 0 5px rgba(245, 232, 73, 0.3), 0 0 6px rgba(245, 232, 73, 0.3);
    }
  }
</style>

<div class="hpny">
    <div class="gradient">
      <h2>
        Happy New Year 2018        
      </h2>
    </div>
    <div class="moons">
      <div class="moon m1"></div>
      <div class="moon m2"></div>
      <div class="moon m3"></div>
      <div class="moon m4"></div>
      <div class="moon m5"></div>
      <div class="moon m6"></div>
      <div class="moon m7"></div>
      <div class="moon m8"></div>
      <div class="moon m9"></div>
      <div class="moon m10"></div>
    </div>
    <div class="stars">
      <div class="star s1"></div>
      <div class="star s2"></div>
      <div class="star s3"></div>
      <div class="star s4"></div>
      <div class="star s5"></div>
      <div class="star s6"></div>
      <div class="star s7"></div>
      <div class="star s8"></div>
      <div class="star s9"></div>
      <div class="star s10"></div>
    </div>
    <div class="chime red">
      <div class="ball">
        <div class="small-ball"></div>
        <div class="small-ball tiny"></div>
      </div>
    </div>
    <div class="chime orange">
      <div class="ball">
        <div class="small-ball"></div>
        <div class="small-ball tiny"></div>
      </div>
    </div>
    <div class="chime blue">
      <div class="ball">
        <div class="small-ball"></div>
        <div class="small-ball tiny"></div>
      </div>
    </div>
    <div class="chime red red2">
      <div class="ball">
        <div class="small-ball"></div>
        <div class="small-ball tiny"></div>
      </div>
    </div>
    <div class="chime orange orange2">
      <div class="ball">
        <div class="small-ball"></div>
        <div class="small-ball tiny"></div>
      </div>
    </div>
  </div>

<template>
  <div class="main-box">
    <div id="ellipse"></div>
    <div id="parallelogram"></div>
    <div id="trapezoid"></div>
    <div id="starFive"></div>
    <div id="starSix"></div>
    <div id="pentagon"></div>
    <div id="hexagon"></div>
    <div id="octagon"></div>
    <div id="heart"></div>
    <div id="infinity"></div>
    <div id="egg"></div>
    <div id="pacman"></div>
    <div id="talkbubble"></div>
    <div id="burst-12"></div>
    <div id="burst-8"></div>
    <div id="diamond"></div>
    <div id="yin-yang"></div>
    <div class="rainbow"></div>
  </div>
</template>

<script>
	export default {
        head: {
            title: 'Icons'
        },
		data () {
			return {}
		}
	}
</script>

<style lang="scss">
  .main-box {
    padding: 50px;
  }

  .main-box>div {
    float: left;
    margin: 10px;
  }

  #ellipse {
    width: 200px;
    height: 100px;
    background-color: red;
    border-radius: 100px/50px;
  }

  #parallelogram {
    margin: 10px;
    width: 200px;
    height: 100px;
    background-color: red;
    transform: skew(150deg);
  }

  #trapezoid {
    margin: 10px 0;
    border-bottom: 100px solid red;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
    width: 100px;
    height: 0px;
  }

  #starFive {
    width: 0;
    height: 0;
    color: red;
    margin: 60px 0;
    position: relative;
    display: block;
    border-left: 100px solid transparent;
    border-right: 100px solid transparent;
    border-bottom: 70px solid red;
    transform: rotate(35deg);
  }

  #starFive::before {
    width: 0;
    height: 0;
    color: red;
    border-left: 30px solid transparent;
    border-right: 30px solid transparent;
    border-bottom: 80px solid red;
    position: absolute;
    top: -47px;
    left: -65px;
    color: white;
    display: block;
    content: "";
    transform: rotate(-35deg);
  }

  #starFive::after {
    width: 0;
    height: 0;
    display: block;
    position: absolute;
    color: red;
    top: 3px;
    left: -105px;
    border-left: 100px solid transparent;
    border-right: 100px solid transparent;
    border-bottom: 70px solid red;
    content: "";
    transform: rotate(-70deg);
  }

  #starSix {
    width: 0;
    height: 0;
    margin-top: 100px;
    border-top: 100px solid red;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
    position: relative;
  }

  #starSix:before {
    width: 0;
    height: 0;
    border-bottom: 100px solid red;
    border-left: 50px solid transparent;
    border-right: 50px solid transparent;
    content: "";
    position: absolute;
    left: -50px;
    top: -135px;
  }

  #pentagon {
    width: 54px;
    height: 0;
    position: relative;
    margin: 50px 0 10px;
    border-width: 50px 18px 0;
    border-style: solid;
    border-color: red transparent;
  }

  #pentagon:before {
    content: "";
    position: absolute;
    width: 0;
    height: 0;
    top: -85px;
    left: -18px;
    border-width: 0 45px 35px;
    border-style: solid;
    border-color: transparent transparent red;
  }

  #hexagon {
    width: 173px;
    height: 100px;
    margin-top: 60px;
    background-color: red;
    position: relative;
  }

  #hexagon::before {
    content: '';
    width: 0;
    height: 0;
    border-bottom: 50px solid red;
    border-left: 86.5px solid transparent;
    border-right: 86.5px solid transparent;
    position: absolute;
    top: -50px;
  }

  #hexagon::after {
    content: "";
    height: 0;
    border-top: 50px solid red;
    border-left: 86.5px solid transparent;
    border-right: 86.5px solid transparent;
    position: absolute;
    bottom: -50px;
  }

  #octagon {
    width: 100px;
    height: 100px;
    background-color: red;
    position: relative;
  }

  #octagon:before {
    width: 42px;
    height: 0;
    top: 0;
    left: 0;
    position: absolute;
    content: "";
    border-left: 29px solid #eee;
    border-right: 29px solid #eee;
    border-bottom: 29px solid red;
  }

  #octagon:after {
    width: 42px;
    height: 0;
    left: 0;
    bottom: 0;
    position: absolute;
    content: "";
    border-left: 29px solid #eee;
    border-right: 29px solid #eee;
    border-top: 29px solid red;
  }

  #heart {
    width: 100px;
    height: 80px;
    position: relative;
  }

  #heart:before,
  #heart:after {
    width: 50px;
    height: 80px;
    left: 50px;
    top: 0;
    background-color: red;
    position: absolute;
    content: "";
    -moz-border-radius: 50px 50px 0 0;
    border-radius: 50px 50px 0 0;
    -webkit-transform: rotate(-45deg);
    -ms-transform: rotate(-45deg);
    -moz-transform: rotate(-45deg);
    -o-transform: rotate(-45deg);
    transform: rotate(-45deg);
    -webkit-transform-origin: 0 100%;
    -ms-transform-origin: 0 100%;
    -moz-transform-origin: 0 100%;
    -o-transform-origin: 0 100%;
    tansform-origin: 0 100%;
  }

  #heart:after {
    left: 0;
    -webkit-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    -moz-transform: rotate(45deg);
    -o-transform: rotate(45deg);
    transform: rotate(45deg);
    -webkit-transform-origin: 100% 100%;
    -ms-transform-origin: 100% 100%;
    -moz-transform-origin: 100% 100%;
    -o-transform-origin: 100% 100%;
    transform-origin: 100% 100%;
  }

  #infinity {
    width: 212px;
    height: 100px;
    position: relative;
  }

  #infinity:before,
  #infinity:after {
    width: 60px;
    height: 60px;
    top: 0;
    left: 0;
    border: 20px solid red;
    position: absolute;
    content: "";
    border-radius: 50px 50px 0 50px;
    -webkit-border-radius: 50px 50px 0 50px;
    -moz-border-radius: 50px 50px 0 50px;
    transform: rotate(-45deg);
    -webkit-transform: rotate(-45deg);
    -ms-transform: rotate(-45deg);
    -moz-transform: rotate(-45deg);
    -o-transform: rotate(-45deg);
  }

  #infinity:after {
    left: auto;
    right: 0;
    border-radius: 50px 50px 50px 0;
    -webkit-border-radius: 50px 50px 50px 0;
    -moz-border-radius: 50px 50px 50px 0;
    transform: rotate(45deg);
    -webkit-transform: rotate(45deg);
    -moz-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    -o-transform: rotate(45deg);
  }

  #egg {
    width: 126px;
    height: 180px;
    background-color: red;
    display: block;
    border-radius: 50% 50% 50% 50%/60% 60% 40% 40%;
    /*-webkit-border-radius:50% 50% 50% 50%/60% 60% 40% 40%;*/
  }

  #pacman {
    width: 0;
    height: 0;
    border-right: 60px solid transparent;
    border-left: 60px solid red;
    border-top: 60px solid red;
    border-bottom: 60px solid red;
    border-top-left-radius: 60px;
    border-top-right-radius: 60px;
    border-bottom-left-radius: 60px;
    border-bottom-right-radius: 60px;
  }

  #talkbubble {
    width: 200px;
    height: 100px;
    background-color: red;
    position: relative;
    border-radius: 10px;
    -webkit-border-radius: 10px;
    -moz-border-radius: 10px;
    -ms-border-radius: 10px;
    -o-border-radius: 10px;
  }

  #talkbubble:before {
    width: 0;
    height: 0;
    right: 100%;
    top: 30px;
    position: absolute;
    content: "";
    border-top: 15px solid transparent;
    border-right: 30px solid red;
    border-bottom: 15px solid transparent;
  }

  #burst-12 {
    width: 80px;
    height: 80px;
    margin-top: 60px;
    background-color: red;
    position: relative;
    text-align: center;
  }

  #burst-12:before,
  #burst-12:after {
    width: 80px;
    height: 80px;
    top: 0;
    left: 0;
    background-color: red;
    position: absolute;
    content: "";
  }

  #burst-12:before {
    transform: rotate(30deg);
    -webkit-transform: rotate(30deg);
    -ms-transform: rotate(30deg);
    -moz-transform: rotate(30deg);
    -o-transform: rotate(30deg);
  }

  #burst-12:after {
    transform: rotate(60deg);
    -webkit-transform: rotate(60deg);
    -ms-transform: rotate(60deg);
    -moz-transform: rotate(60deg);
    -o-transform: rotate(60deg);
  }

  #burst-8 {
    width: 80px;
    height: 80px;
    background-color: red;
    text-align: center;
    position: relative;
    transform: rotate(20deg);
    -webkit-transform: rotate(20deg);
    -ms-transform: rotate(20deg);
    -moz-transform: rotate(20deg);
    -o-transform: rotate(20deg);
  }

  #burst-8:before {
    width: 80px;
    height: 80px;
    top: 0;
    left: 0;
    background-color: red;
    position: absolute;
    content: "";
    transform: rotate(135deg);
    -webkit-transform: rotate(135deg);
    -ms-transform: rotate(135deg);
    -moz-transform: rotate(135deg);
    -o-transform: rotate(135deg);
  }

  #diamond {
    width: 50px;
    height: 0;
    border-style: solid;
    border-color: transparent transparent red transparent;
    border-width: 0 25px 25px 25px;
    position: relative;
    margin: 20px 0 50px 0;
  }

  #diamond:after {
    width: 0;
    height: 0;
    top: 25px;
    left: -25px;
    border-style: solid;
    border-color: red transparent transparent transparent;
    border-width: 70px 50px 0 50px;
    position: absolute;
    content: "";
  }

  #yin-yang {
    width: 96px;
    height: 48px;
    background-color: #fff;
    border-color: red;
    border-style: solid;
    border-width: 2px 2px 50px 2px;
    border-radius: 100%;
    position: relative;
  }

  #yin-yang::before {
    width: 12px;
    height: 12px;
    top: 50%;
    left: 0;
    content: "";
    position: absolute;
    background-color: #fff;
    border: 18px solid red;
    border-radius: 100%;
  }

  #yin-yang::after {
    width: 12px;
    height: 12px;
    top: 50%;
    left: 50%;
    background-color: red;
    border: 18px solid #fff;
    border-radius: 100%;
    content: "";
    position: absolute;
  }
  .rainbow {
    width: 200px;
    height: 100px;
    border-radius: 100px 100px 0 0;
    background-color: #7367f3;
    overflow: hidden;
  }
  .rainbow::after {
    width: 200px;
    height: 200px;
    display: block;
    content: "";
    background: -webkit-radial-gradient(farthest-side, #fff 50%, #f0f, #00f, #0ff, #0f0, #ff0, #f00); /* Safari 5.1 - 6.0 */
    background: -o-radial-gradient(farthest-side, #fff 50%, #f0f, #00f, #0ff, #0f0, #ff0, #f00); /* Opera 11.6 - 12.0 */
    background: -moz-radial-gradient(farthest-side, #fff 50%, #f0f, #00f, #0ff, #0f0, #ff0, #f00); /* Firefox 3.6 - 15 */
    background: radial-gradient(farthest-side, #fff 50%, #f0f, #00f, #0ff, #0f0, #ff0, #f00); /* 标准的语法 */    
  }	
</style>

<template>
  <div id="app">
    <Load></Load>

    <Banner></Banner>

    <LineWords></LineWords>

    <Can :quan="quan" :qiyong="qiyong" :num="num"></Can>

    <p class="jiaLine">sd**2被好朋友加油，抵现券起用金额降至35000元</p>

    <Benefit></Benefit>

    <Foot></Foot>
  </div>
</template>

<script>
import Loading from './components/Loading.vue'
import Banner from './components/Banner.vue'
import Line from './components/Line.vue'
import Can from './components/Can.vue'
import Benefit from './components/Benefit.vue'
import Foot from './components/Foot.vue'


export default {
  name: 'app',

  mounted: function() {
    // console.log(1)
  },

  components: {
    Load: Loading,
    Banner: Banner,
    LineWords: Line,
    Can: Can,
    Benefit: Benefit,
    Foot: Foot,
  },

  data: function () {
    return {
      quan: '300',
      qiyong: '37000',
      num: 3,
    }
  }
}
</script>

<style>
html,body,h1,h2,h3,h4,h5,h6,div,dl,dt,dd,ul,ol,li,p,blockquote,pre,hr,figure,table,caption,th,td,form,fieldset,legend,input,button,textarea,menu{margin:0;padding:0;box-sizing:border-box;-webkit-box-sizing:border-box;}
html,body,form,fieldset,p,div,h1,h2,h3,h4,h5,h6{-webkit-text-size-adjust:none}
html{font-size:16px}
body{font-family:"微软雅黑",arial,sans-serif; background:#e6e6e6;}
header,footer,section,article,aside,nav,hgroup,address,figure,figcaption,menu,details{display:block;}
table{border-collapse:collapse;border-spacing:0;}
caption,th{text-align:left;font-weight:normal;}
html,body,fieldset,img,iframe,abbr{border:0;}
i,cite,em,var,address,dfn{font-style:normal;}
[hidefocus],summary{outline:0;}
li{list-style:none;}
h1,h2,h3,h4,h5,h6,small{font-size:100%;font-style: normal;font-weight: normal;}
sup,sub{font-size:83%;}
pre,code,kbd,samp{font-family:inherit;}
q:before,q:after{content:none;}
textarea{overflow:auto;resize:none;}
label,summary{cursor:default;}
a,button{cursor:pointer;border:none;}
del,ins,u,s,a,a:hover{text-decoration:none;}
body,textarea,input,button,select,keygen,legend{color:#333;outline:0;}
body *{-webkit-tap-highlight-color:rgba(0,0,0,0);tap-highlight-color:rgba(0,0,0,0)}
.clearfix:after{content:".";display:block;overflow:hidden;height:0;clear:both;visibility:hidden;}
* html .clearfix{height:1%;}
input,textarea,select{outline: none; -webkit-appearance:none;}
.clearOver{overflow: hidden; text-overflow:ellipsis; white-space: nowrap;}
.floatL{ float: left;}
.floatR{ float: right;}
@media screen and (min-width: 320px) { html { font-size: 13.653333px; } }
@media screen and (min-width: 375px) { html { font-size: 16px; } }
@media screen and (min-width: 414px) { html { font-size: 17.664px; } }

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #f4e8d8;
  width: 100%;
}

.jiaLine {
  font-size: .875rem;
  line-height: 3;
  background-image: linear-gradient(to right, transparent 0, #e4d5c0 30%, #e4d5c0 70%, transparent 100%);
}
</style>

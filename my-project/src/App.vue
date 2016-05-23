<template>
  <div transition="app">
    <div class="clearfix pageleft">
        <pagenav></pagenav>
    </div>
    <div class="pageright" id='pagecontent'>
         <router-view></router-view>
    </div>
  </div>
</template>

<script>
import pagenav from './components/nav'
// var Components = {
//   pagenav
// }
// module.exports = Components
export default {
  components:{pagenav}
}
// export default {
//   components:{hello}
// }
// export default {
//   components:{pagenav}
// }
</script>

<style>
#app{
    min-height: 1000px;
}
.pageleft{
    width: 200px;
    position: fixed;
    top: 0;
    left: 0px;
    overflow-x: hidden;
    overflow-y: auto;
    padding:20px;
    background-color: #013A77;
    min-height: 1000px;
}
.pageright{
    margin-left: 240px;
    background:url('assets/bg.jpg') repeat-y;
    min-height: 1000px;
    background-size: cover;
}
.nav{
    color: #fff;
}
.nav .cat1{
    font-size: 25px;
    font-weight: bold;

}
.nav .cat2 a{
    display: inline-block;
    padding-top: 15px;
    font-size: 18px;
    color: #fff;
}
.nav .cat2 a:hover{
   text-decoration: underline;
}
</style>

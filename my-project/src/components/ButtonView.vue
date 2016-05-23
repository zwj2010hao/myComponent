<template>
   <div class="wrap">
        <article class="clearfix">
            <h2>Button &lta&gt</h2>
            <div class="section fl">
                <a href="javascript:void(0)" class="btn btn-class1">button</a>
            </div>
            <div class="section fl">
                <a href="javascript:void(0)" class="btn btn-disabled">Disabled button</a>
            </div>
        </article>
        <article class="clearfix">
            <h2>Button &ltbutton&gt</h2>
            <div class="section fl">
                <button class="button btn-class1">button</button>
            </div>
            <div class="section fl">
                <button class="button btn-disabled" disabled="disabled">Disabled button</button>
            </div>
        </article>
        <article class="clearfix">
            <h2>Other (use tag a)</h2>
            <div class="section fl">
                <i class="iconfont">&#xe65a;</i>
                <a href="javascript:void(0)" class="btn btn-class1">button</a>
            </div>
        </article>
   </div>
</template>

<script>
export default {
    data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg:'button widget'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
@import "./style/widget/button.scss";
@import "../assets/font/iconfont.css";
</style>

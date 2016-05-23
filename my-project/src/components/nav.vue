<template>
    <ul class="nav">
        <li v-for="item in navMsg" class="cat1">
            {{item.category}}
            <ul>
                <li v-for="item in item.cates" class="cat2">
                   <a v-link="{path: '/'+item.url}">{{item.name}}</a>
                </li>
            </ul>
        </li>
    </ul>
</template>

<script>
export default {
    data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      navMsg: [
        {
            category:'pc',
            cates:[{
                name:'button',
                url:'button'
            },{
                name:'类别2',
                url:'aa'
            },{
                name:'类别3',
                url:'aa'
            }]
          },{
            category:'m',
            cates:[{
                name:'类别1',
                url:'aa'
            },{
                name:'类别2',
                url:'aa'
            },{
                name:'类别3',
                url:'aa'
            }]
          }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}
</style>

<template>
  <div class="btn">
    <button @click="handle">{{text}}</button>
  </div>
</template>

<script>
export default {
  name: 'btn', // 组件的name属性（后面有提到这里有个坑）
  props: {
    text: { // 文本
      type: String,
      default () {
        return ''
      }
    }
  },
  data () {
    return {
    }
  },
  methods:{
    handle(){
      alert('我点击了')
    }
  }
}
</script>
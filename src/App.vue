<template>
  <div>
    <button @click="change">点击</button>
      <span>
        {{active}}
      </span>
  </div>
</template>

<script>
export default {
  
  data(){
    return {
      active:1,
    }
  },
  mounted(){
  },
  methods:{
    change(){
      switch (this.active) {
        case 1:
          this.active = '我在第一个'
          break;
        case 2:
          this.active = '我在第二个'
          break;
        case 3:
          this.active = '我在第三个'
          break;
      }
    }
    
  }
}
</script>

<style>
</style>
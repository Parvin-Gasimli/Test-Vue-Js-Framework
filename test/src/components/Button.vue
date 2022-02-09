<template>
  <button @click="onClick()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods:{
      onClick(){
          console.log('cliked')
      },
  }
};
</script>
<style scoped>
.btn {
    margin-top: 25px;
    margin-right: 5px;
  width: 200px;
  height: 30px;
  border: none;
  color: white;
}
</style>

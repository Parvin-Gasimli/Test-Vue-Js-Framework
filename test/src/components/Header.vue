<template>
  <header>
    <h1>{{title}}</h1>
    <Button text="Add Task" color="black"/>
  
   
  </header>
</template>

<script>
import  Button from './Button'
export default {
 
  name: "Header",
  props:{
      title:{
          type:String,
          default:'Hello Code'
      }
  },
  components:
  {
    Button
  }
};
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
}
</style>
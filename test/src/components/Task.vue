<template>
 <div class="task">
 <h3>     {{task.text}}</h3>
 <p>{{task.day}}</p>
 </div>
</template>


<script>
import Task from './Task'
export default {
    name:'Task',
    props:{
        task:Object
    },
    components:{
        Task
    }
}
</script>


<style scoped>
.task{
    background: #f4f4f4;
    margin: 5px;
    padding: 10px 20px;
    cursor: pointer;
}

.task .reminder{
    border-left: 5px solid green;
}
</style>
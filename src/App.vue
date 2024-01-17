<script setup>
import { ref} from 'vue';
const tasks = ref([{
    name: 'Task 1',
    time: 30
}, {
    name: 'Task 2',
    time: 40
}, {
    name: 'Task 3',
    time: 60
}, {
    name: 'Task 4',
    time: 45
}, {
    name: 'Task 5',
    time: 50
}]);


</script>

<template>
  <div>

    <div>
      <h2>This is Task Manager</h2>
    </div>
    <div  v-for="(task,index) in tasks" :key="index" class="flex item-center justify-center m-5">
        <p class="mr-5">{{ index+1 }}</p>
        <p class="mr-5">{{ task.name }}</p>
        <p class="mr-5">{{ task.time }}</p>
        <Button class="">Update</Button>
    </div>

    
   </div>

 
   
</template>

<style scoped>

</style>

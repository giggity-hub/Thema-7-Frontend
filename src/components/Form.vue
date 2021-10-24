<script >
import {ref} from 'vue';
import 'axios'
// const descrconstiption = ref("")
// const title = ref("")


// function submit(){
//     console.log(title,description);
// }

export default {
  data() {
    return {
      description: "",
      title: "",
    };
  },
  methods: {
    submit() {
    console.log(this.title); // logs the input value
    },
  },
};
</script>

<template>

    <div id="form" class="bg-red-500 w-full max-w-3xl p-4">
        <h3 class="label">Title</h3>
        <input v-model="title" class="text-input" type="text" name="" id="">

        <h3 class="label">Description</h3>
        <textarea v-model="description" class="text-input" name="" id="" cols="30" rows="10"></textarea>

        <button @click="submit" class="btn btn-blue my-3 ">Submit</button>
    
    </div>
</template>

<style scoped>

.text-input{
    @apply bg-gray-400 rounded w-full 
}
.label{
    @apply text-white py-3
}

.btn {
    @apply font-bold py-2 px-4 rounded;
}
.btn-blue {
@apply bg-blue-500 text-white;
}
.btn-blue:hover {
@apply bg-blue-700;
}
</style>
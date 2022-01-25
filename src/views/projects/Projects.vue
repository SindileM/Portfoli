<template>
    <h1>This is my projects page</h1>
      <div v-for="project in projects" :key="project.id" class="job">
          <router-link :to="{ name:'ProjectDetails', params: {id: job.id }}" 
             <h2>{{ project.title }}</h2> 
          </router-link> 
          </div>
        </div>  
</template>

<script>
export default {
    data() {
        return {
            projects:[]
        }
    }
    // mounted() {
    //     fetch('')
    //     .then(res => res.json())
    //     .then(data => this.projects = data)
    //     .catch(err => console.log(err.message))
    // },
}
</script>
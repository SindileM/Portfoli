<template>
    <div v-if="project">
        <h1>{{ project.title}}</h1>
        <p>The project id is {{ id }}</p>
        <h1>{{ project.details }}</h1>
    </div> 
    <div v-else>
        <p>Loading project data...</p>
    </div>       
</template>
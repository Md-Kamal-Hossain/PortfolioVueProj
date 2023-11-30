
<template>

<div class="main-container">
    <div v-for="(project, index) in projectData.ProjectsArray" :key="index" class="project-card">
      <h2>{{ project.Title }}</h2>
      <img src="../assets/cup.png" alt="">
      <p>{{ project.About }}</p>
      <div class="links">
        <a :href="project.Link1" target="_blank"><img src="../assets/github.png" alt=""></a>
        <a :href="project.Link2" target="_blank"><img src="../assets/link.png" alt=""></a>
      </div>
    </div>
  </div>



  
</template>

<script>
import jsonData from "/projects.json"
export default {
    data(){
        return{
            projectData: jsonData
        }
    }

}
</script>

<style scoped>

.main-container{
    margin-top: 4%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    height: 10rem;
    
    
    
}
.project-card{
    margin: 5px;
  padding: 30px;
  flex: 0 0 30%; /* Set a fixed width for your project cards (adjust as needed) */
  background-color: #cca0a0;
  border-radius: 20px;
  box-shadow: none;
  height: 15rem;
  
}
.project-card img{
  height: 5rem;
  width: 100%; /* Ensure the image takes the full width of the project card */
  border-radius: 15px; /* Adjust as needed */
}
.links {
  display: flex;
  flex-direction: row;
  align-items: flex-end; /* Align items to the bottom */
  justify-content: flex-end; /* Align items to the right */
}

.links img {
  height: 2rem;
  margin: 5px;
}


</style>
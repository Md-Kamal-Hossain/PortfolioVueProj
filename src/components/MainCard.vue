<template>
  <div class="wrapper">
    <div class="main-container">
    <div class="container-one">
        <div class="profile">
            <img src="../assets/cup.png" alt="">
            <h3>Kamal Hossain</h3>
            <p>Software Developer</p>
        </div>
        <div class="social-link">
            
                <div class="link">
                    <img src="https://avatars.githubusercontent.com/<username>" alt="GitHub Avatar">
                    <a href=""><h2> Github </h2></a>
                </div>
                <div class="link">
                    <img src="../assets/twitter.png" alt="">
                    <a href=""><h2> Twiter </h2></a>
                </div>
                <div class="link">
                    <img src="../assets/linkedin.png" alt="">
                    <a href=""><h2> LinkedIn </h2></a>
                </div>
                <div class="link">
                    <img src="../assets/xing.png" alt="">
                    <a href=""><h2> Xing </h2></a>
                </div>
            
        </div>
    </div>
    <div class="container-two">
        <div class="about-me">
            <h1> About Me</h1>
            <p>Lorem ipsum dolor sit amet consectetur,
             adipisicing elit. Rerum deserunt corrupti 
             ab officia, veniam doloribus quos quam 
             temporibus? Qui rerum non quaerat deserunt 
             mollitia? Quis asperiores reiciendis accusamus
              officiis neque.
            </p>

        </div>
        <div class="technology-section">
            <h1>
                Technology Studied
            </h1>
            <div class="logos">
                <img src="../assets/js.png" alt="">
                <img src="../assets/html1.png" alt="">
                <img src="../assets/css1.png" alt="">

            </div>
        </div>
        <div class="button-container">
    <div class="projects-button">
        <div>
            <a href="">My Projects</a>
        </div>
    </div>
    <div class="projects-button">
        <div>
            <a href="">My Resume</a>
        </div>
    </div>
</div>
    </div>
  </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.wrapper{
    display: flex;
    justify-content: center;
}
img{
    height:20px;
}
.main-container{
    display:flex;
    flex-direction: row;
    background-color: gainsboro;
    border-radius: 25px;
}
.container-one{
    background-color: aqua;
    padding: 3%;
    
    width: 35%;
    border-radius: 25px;
}

.profile img{
    height: 5.5rem;
    border-radius: 50%;
}
.link a{
    text-decoration: none;
    color: #2c3e50;
    font-size: 12px;
}
.link img{
    height: 3rem;
}
.container-two{
    background-color: blueviolet;
    
    width:65% ;
    border-radius: 5px;
    
}
.about-me {
    text-align: left;
}
.logos img{
    height:3rem;
}
.button-container{
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
.projects-button {
    background-color: #2c3eff;
    margin: 5px;
    padding: 2px;
    border-radius: 5px; /* Adding rounded corners for a nice look */
}

.projects-button a {
    text-decoration: none;
    color: #2c3e55;
    padding: 2px;
}
@media only screen and (max-width:950px){
    .main-container{
        width: 95%;
    }
}

</style>
<template>
  <div>
    <h1>Projects</h1>
  </div>
  <div class="project-container">
    <div class="project-1 project-space">
      <img img src="/images/portfolio-pic-1.jpeg" width="200" alt="project-1.jpg">
      <div class="project-details">
        <h3>Ticket Management Web App</h3>
        <p>In my second year of the BIS Multimedia program, I developed a ticket management web application as part of an assignment. The app enables users to create tickets for any queries or issues they encounter. It efficiently queues and manages these tickets, providing a streamlined system for tracking and resolving user concerns.</p>
        <p class="tech-stack">Tech Stack: Vue Framework, CSS</p>
      </div>
    </div>
    <div class="project-2 project-space">
      <img src="/images/portfolio-pic-2.png" width="200" alt="project-2.jpg">
      <div class="project-details">
        <h3>Comic Project</h3>
        <p>In my first year, I was tasked with creating an original comic from start to finish. This project helped me learn and apply design principles, art elements, and storytelling techniques.</p>
        <p class="tech-stack">Tech Stack: Adobe Illustrator</p>
      </div>
    </div>
    <div class="project-3 project-space">
      <img src="/images/portfolio-pic-3.jpeg" width="200" alt="project-3.jpg">
      <div class="project-details">
        <h3>Twine Interactive Web Story</h3>
        <p>In my second year, I created an interactive web story using Twine. The project allowed users to choose their own paths within the narrative, with their decisions directly influencing the story’s outcome.</p>
        <p class="tech-stack">Tech Stack: Twine</p>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style scoped>
  h1 {
    margin-top: 4rem;
    text-align:center;
  }

  .project-space {
    display:flex;
    justify-content:space-between;
    margin:3rem 0rem;
    align-items:center;
  }

  .project-space div, .project-space img {
    margin: 0px 30px;
  }

  .tech-stack {
    color:#e9c46a;
  }

  .project-container {
    padding-bottom: 50px; 
  }

  img {
    border-radius: 10px
  }

</style>
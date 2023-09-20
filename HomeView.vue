<template>
  <div>
    <header>
      <h1>Welcome to My Portfolio</h1>
    </header>
    <main>
      <section class="intro">
        <h2>Hello, I'm Saksham</h2>
        <p>Welcome to my portfolio website. I'm a web developer passionate about creating user-friendly and visually appealing websites. Explore my projects below.</p>
      </section>
      <section class="featured-projects">
        <h2>Featured Projects</h2>
        <div class="project-card">
          <h3>Project 1</h3>
          <p>This is an imaginary project description.</p>
        </div>
        <div class="project-card">
          <h3>Project 2</h3>
          <p>Another imaginary project description.</p>
        </div>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>

<style scoped>
/* Specific styles for the home page */
.intro {
  background-color: pink;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 2rem;
  text-align: center;
}

.intro h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

.intro p {
  font-size: 1rem;
  line-height: 1.5;
}

.featured-projects {
  margin-top: 2rem;
}

.project-card {
  background-color: plum;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 1rem;
  margin-bottom: 2rem;
  text-align: center;
}

.project-card img {
  max-width: 100%;
  height: auto;
}

.project-card h3 {
  font-size: 1.25rem;
  margin-top: 1rem;
}

.project-card p {
  font-size: 1rem;
  margin-top: 0.5rem;
}

</style>



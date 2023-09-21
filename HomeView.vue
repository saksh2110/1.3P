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
        <div class="project-card" v-for="project in projects" :key="project.id">
          <img :src="project.image" :alt="project.title">
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
        </div>
      </section>
      <section class="contact-form">
        <h2>Contact Me</h2>
        <form>
          <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
          </div>
          <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
          </div>
          <div class="form-group">
            <label for="message">Message:</label>
            <textarea id="message" name="message" rows="4" required></textarea>
          </div>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Project 1",
          description: "This is an imaginary project description. Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
          image: "project1.jpg",
        },
        {
          id: 2,
          title: "Project 2",
          description: "Another imaginary project description. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
          image: "project2.jpg",
        },
      ],
    };
  },
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
  background-color: palevioletred;
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

/* Form styles */
.contact-form {
  background-color: white;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 2rem;
  margin-top: 2rem;
}

.contact-form h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

.form-group {
  margin-bottom: 1rem;
}

.form-group label {
  display: block;
  font-size: 1rem;
  margin-bottom: 0.5rem;
}

.form-group input[type="text"],
.form-group input[type="email"],
.form-group textarea {
  width: 100%;
  padding: 0.5rem;
  font-size: 1rem;
  border: 1px solid white;
  border-radius: 5px;
}

.form-group textarea {
  resize: vertical;
}

button[type="submit"] {
  background-color: blue;
  color: white;
  border: none;
  border-radius: 5px;
  padding: 0.5rem 1rem;
  font-size: 1rem;
  cursor: pointer;
}

button[type="submit"]:hover {
  background-color: blue;
}
</style>

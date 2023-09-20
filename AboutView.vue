<template>
  <div>
    <header>
      <h1>About Me</h1>
    </header>
    <main>
      <section class="about-me">
        <h2>Who I Am</h2>
        <p>I am a passionate web developer with a creative mind and a keen eye for detail. My journey into the world of web development started when I built my first website at the age of 16, and I've been hooked ever since. I specialize in front-end development, creating user-friendly and visually appealing web experiences.</p>
      </section>
      <section class="skills">
        <h2>Skills</h2>
        <ul>
          <li>HTML5 &amp; CSS3</li>
          <li>JavaScript (ES6+)</li>
          <li>Vue.js &amp; React</li>
          <li>Responsive Web Design</li>
          <li>UI/UX Design</li>
          <li>Version Control (Git)</li>
        </ul>
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
/* Specific styles for the about section */
.about-me {
  background-color: skyblue;
  border-radius: 10px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 2rem;
}

.about-me h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

.about-me p {
  font-size: 1rem;
  line-height: 1.5;
}

.skills ul {
  list-style-type: disc;
  padding-left: 1rem;
}

.skills li {
  font-size: 1rem;
  margin-top: 0.5rem;
}
</style>

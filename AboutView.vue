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
      <section class="experience">
        <h2>Work Experience</h2>
        <table>
          <thead>
            <tr>
              <th>Position</th>
              <th>Company</th>
              <th>Year</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Front-end Developer</td>
              <td>ABC Web Solutions</td>
              <td>2020-2022</td>
            </tr>
            <tr>
              <td>UI/UX Designer</td>
              <td>XYZ Design Studio</td>
              <td>2018-2020</td>
            </tr>
          </tbody>
        </table>
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
  name: "About",
};
</script>

<style scoped>
/* Specific styles for the about section */
.about-me {
  background-color: beige;
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

/* Table styles */
.experience {
  margin-top: 2rem;
}

table {
  width: 100%;
  border-collapse: collapse;
  margin-top: 1rem;
  border: 1px solid black; /* Add a border to the entire table */
}

table th,
table td {
  padding: 0.5rem;
  text-align: left;
  border-bottom: 1px solid black; /* Add a border to table headers and data cells */
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
  border: 1px solid black;
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

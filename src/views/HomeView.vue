<template>
  <section class="home">
    <header class="hero">
      <h1>Welcome to My Portfolio</h1>
      <p>Cybersecurity Analyst</p>
      <router-link to="/projects" class="cta-button">Explore My Work</router-link>
    </header>

    <section class="about-me">
      <h2>About Me</h2>
      <p>
        Greetings, I'm Johann Ogbebor, a dedicated Cybersecurity Analyst with a strong background in safeguarding digital assets and ensuring the integrity of sensitive information. With over 3 years of experience in identifying and mitigating security threats, I'm committed to protecting your organization from cyber risks. Let's fortify your digital defenses together!
      </p>

    </section>

    <section class="contact">
      <h2>Contact Me</h2>
      <p>Feel free to reach out to me via email:</p>
      <a href="mailto:johann@gmail.com" class="email-link">johann@gmail.com</a>
    </section>
  </section>
</template>

<script setup>

</script>

<style scoped>
/* Define styles specific to the home page */
.home {
  font-family: 'Arial', sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

.hero {
  text-align: center;
  margin-bottom: 50px;
  background-image: url('C:\Users\johan\OneDrive - Deakin University\Assignments\Trimester 2\Introduction to Responsive Web Apps\Task 1.3\src\assets\images\bg.jpg');
  background-size: cover;
  background-position: center;
  color: #fff;
  padding: 100px 0;
}

.hero h1 {
  font-size: 2.5em;
  margin-bottom: 10px;
}

.cta-button {
  display: inline-block;
  background-color: #6f7173;
  color: #fff;
  padding: 10px 20px;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
  transition: background-color 0.3s;
}

.cta-button:hover {
  background-color: #6f7173;
}

.about-me {
  text-align: center;
  margin-bottom: 50px;
}

.contact {
  text-align: center;
  margin-bottom: 50px;
}

.email-link {
  color: #6f7173;
  text-decoration: none;
  font-weight: bold;
  margin-left: 5px;
}

.email-link:hover {
  text-decoration: underline;
}
</style>

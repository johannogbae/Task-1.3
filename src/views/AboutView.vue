<template>
  <section class="about-me-page">
    <div class="about-content">
      <h1>About Me</h1>
      <p>
        Greetings! I'm Johann Ogbebor, a Cybersecurity Analyst deeply dedicated to safeguarding digital landscapes from potential threats. With a strong foundation in web development spanning 3 years, I possess a unique perspective on security, leveraging state-of-the-art technologies to fortify your digital defenses.
      </p>
      <p>
        My journey began at Deakin University, where I pursued my passion in Information technology major in Cybersecurity, acquiring essential skills in cybersecurity along the way. Since then, I've partnered with diverse clients and organizations, delivering robust cybersecurity solutions that ensure peace of mind.
      </p>
      

      <div class="cta-section">
        <a href="/projects" class="cta-button">Explore My Work</a>
        <a href="mailto:your-email@example.com" class="cta-button">Get in Touch</a>
      </div>
    </div>
    <div class="profile-image">
      <img src="../assets/images/profilepic.jpg" alt="Johann Ogbebor" class="hover-effect">
    </div>
  </section>
</template>

<script setup>

</script>

<style scoped>
.about-me-page {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 40px 0;
  font-family: 'Arial', sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  background-color: #f8f8f8;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.about-content {
  flex: 2;
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
}

.about-content h1 {
  font-size: 2.5em;
  margin-bottom: 20px;
}

.about-content p {
  margin-bottom: 20px;
  line-height: 1.6;
}

.cta-section {
  display: flex;
  gap: 20px;
  margin-top: 20px;
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

.profile-image {
  flex: 1;
  padding-left: 50px;
}

.profile-image img.hover-effect {
  max-width: 100%;
  border-radius: 90%;
  transition: transform 0.3s, box-shadow 0.3s;
}

.profile-image img.hover-effect:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}
</style>

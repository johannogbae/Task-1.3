<template>
    <section class="my-portfolio">
      <h2>My Projects</h2>
      <div class="portfolio-items">
        <div class="portfolio-item" v-for="project in projects" :key="project.id">
          <div class="portfolio-image">
            <img :src="project.image" :alt="project.name" />
          </div>
          <div class="portfolio-details">
            <h3>{{ project.name }}</h3>
            <p>{{ project.description }}</p>
            <a :href="project.url" class="btn-link">View Project</a>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const projects = ref([
    {
      id: 1,
      name: 'Project 1',
      description: 'Web development for Uber.',
      image: '@/assets/images/project1.jpg',
      url: 'https://www.example.com/project-alpha'
    },
    {
      id: 2,
      name: 'Project 2',
      description: 'Protection against cyber threat.',
      image: '@/assets/images/project2.jpg',
      url: 'https://www.example.com/project-beta'
    },
    
  ]);
  </script>
  
  <style scoped>
  .my-portfolio {
    font-family: 'Arial', sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .portfolio-items {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  
  .portfolio-item {
    flex: 1;
    border: 1px solid #e0e0e0;
    border-radius: 8px;
    overflow: hidden;
    transition: transform 0.3s;
  }
  
  .portfolio-item:hover {
    transform: scale(1.03);
  }
  
  .portfolio-image img {
    width: 100%;
    height: auto;
  }
  
  .portfolio-details {
    padding: 20px;
  }
  
  .portfolio-details h3 {
    font-size: 1.5em;
    margin-top: 0;
  }
  
  .btn-link {
    display: inline-block;
    background-color: #6f7173;
    color: #fff;
    padding: 10px 20px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s;
  }
  
  .btn-link:hover {
    background-color: #6f7173;
  }
  </style>
  
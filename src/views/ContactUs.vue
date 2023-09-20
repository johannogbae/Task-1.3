<template>
  <div class="contact-page">
    <h2>Contact Me</h2>
    <div class="contact-details">
      <div class="contact-info">
        <h3>Contact Information</h3>
        <p>Email: johann@gmail.com</p>
        <p>Phone: +1 (123) 456-7890</p>
        <p>Address: 12 Main Street, Melbourne, Australia</p>
      </div>
      <div class="feedback-form">
        <h3>Send Feedback</h3>
        <form @submit.prevent="handleSubmit">
          <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" v-model="formData.name" required />
          </div>

          <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" v-model="formData.email" required />
          </div>

          <div class="form-group">
            <label for="message">Message:</label>
            <textarea id="message" v-model="formData.message" required></textarea>
          </div>

          <button type="submit">Submit</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const formData = ref({
  name: '',
  email: '',
  message: ''
});

const handleSubmit = () => {
  console.log(formData.value);

  // Reset the form
  formData.value = {
    name: '',
    email: '',
    message: ''
  };
};
</script>

<style scoped>
.contact-page {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

.contact-details {
  display: flex;
  justify-content: space-between;
  gap: 20px;
}

.contact-info,
.feedback-form {
  flex: 1;
}

.contact-info h3,
.feedback-form h3 {
  font-size: 1.5em;
  margin-bottom: 10px;
}

.contact-info p {
  margin: 0 0 10px;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 10px;
}

input[type="text"],
input[type="email"],
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  padding: 10px 15px;
  background-color: #6f7173;
  color: #fff;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #6f7173;
}
</style>

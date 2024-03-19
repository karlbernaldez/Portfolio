<template>
    <section class="contact">
      <div class="container">
        <h2 class="section-title">Get in Touch</h2>
        <form @submit.prevent="submitForm">
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" id="name" v-model="name">
          </div>
          <button type="submit" class="btn-primary">Send Message</button>
        </form>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        // ... other form fields
      };
    },
    methods: {
      submitForm() {
        // Handle form submission logic (e.g., send data to an API)
        console.log('Form submitted:', this.name); 
      }
    }
  }
  </script>
  
  <style scoped>
  /* Styles for .contact, form elements, etc. */
  </style>
  
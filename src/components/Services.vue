<template>
    <section class="services">
      <div class="container">
        <h2 class="section-title">My Services</h2>
        <div class="services-list">
          <div class="service-item" v-for="service in services" :key="service.id">
            <h3>{{ service.title }}</h3>
            <p>{{ service.description }}</p>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        services: [
          { id: 1, title: 'Web Development', description: 'Crafting modern websites...' },
          { id: 2, title: 'Mobile App Development', description: 'Building engaging mobile experiences...' },
          // Add your other services here
        ]
      };
    }
  }
  </script>
  
  <style scoped>
  /* Styles for .services, .services-list, .service-item */
  </style>
  
<template>
  <div id="app">
    <vue-particles id="tsparticles" :options="options"/>
    <Header />
    <main>
      <Hero /> 
      <About id="about" />
      <Projects />
      <Contact />
    </main>
    <footer class="footer">
        &copy; {{ currentYear }} Adovelopers
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Hero from './components/Dashboard.vue';
import About from './components/About.vue';
import Services from './components/Services.vue';
import Contact from './components/Contact.vue';
import Projects from './components/Projects.vue';


export default {
  name: 'App',
  components: {
    Header,
    Hero,
    About,
    // Projects
  },
  data() {
    return {
      currentYear: new Date().getFullYear()
    }
  },
  mounted() {
    // Smooth scrolling when clicking on anchor links
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      anchor.addEventListener('click', function (e) {
        e.preventDefault();

        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
          const options = {
            behavior: 'smooth',
            block: 'start', // Adjust alignment as needed ('start', 'center', 'end', or 'nearest')
          };
          target.scrollIntoView(options);
        }
      });
    });
  }
}

</script>

<style>
#app {
  @import './style.css'; 
}

/* Add global styles if needed */
</style>./components/karl/About.vue./components/karl/Contact.vue./components/karl/Dashboard.vue./components/karl/Header.vue./components/karl/Services.vue./components/About.vue./components/Contact.vue./components/Dashboard.vue./components/Header.vue./components/Services.vue

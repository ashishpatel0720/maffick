<template>
  <div class="tc-about">
    <p class="tc-about-text" style="font-family:Comfortaa,cursive,'DejaVu Sans'">
      The Wait Is Finally Over! <br>
      <span class="tc-about-special coral">NIT Bhopal</span> proudly brings you the latest instalment of <br>Central India's Largest Cultural Fest!
      <span class="tc-about-special someblue">Maffick'18</span>
    </p>
  </div>
</template>

<script>
  import ScrollReveal from 'scrollreveal';
  export default {
    name: 'About',
    mounted() {
      window.sr = ScrollReveal({
        reset: true,
        duration: 1000
      });
      sr.reveal('.tc-about-text')
    }
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .tc-about {
    padding: 5%;
  }
  .tc-about-text {
    font-family: 'Source Sans Pro', Serif;
    font-size: 35px;
    font-weight: bold;
    color: #e0e0e0;
  }
  .coral {
    color: #ff7f50;
  }
  .someblue {
    color: #00d1b2;
  }

  @media only screen and (max-width: 500px) {
    .tc-about-text {
      font-size: 24px;
    }
  }
</style>

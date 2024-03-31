<!-- Header.svelte -->

<script>
    export let name = "Omid Abdi";
    export let tagline = "Empowering learners for 25 years";
  </script>
  
  <header class="header">
    <h1 class="title">{name}</h1>
    <p class="tagline">{tagline}</p>
  </header>
  
  <style>
    .header {
      background-color: #333; /* Dark background color */
      color: #fff; /* White text color */
      padding: 20px;
      text-align: center;
    }
  
    .title {
      font-size: 2em;
      margin-bottom: 0.5em;
    }
  
    .tagline {
      font-size: 1.2em;
      opacity: 0.8; /* Slightly reduced opacity for tagline */
    }
  </style>
  
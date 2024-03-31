<!-- Introduction.svelte -->

<script>
    export let introduction = "Welcome to my webpage! I am Omid Abdi, a Cambridge CELTA certified teacher with 25 years of experience. Throughout my career, I have been dedicated to empowering learners and fostering a supportive learning environment. I believe in personalized instruction tailored to each student's needs, ensuring a rewarding learning experience for all. I'm excited to share my passion for teaching with you!";
  </script>
  
  <section class="introduction">
    <div class="content">
      <p>{introduction}</p>
    </div>
  </section>
  
  <style>
    .introduction {
      padding: 20px;
      text-align: center;
    }
  
    .content {
      max-width: 800px;
      margin: 0 auto;
    }
  
    /* Responsive styles */
    @media (max-width: 768px) {
      .content {
        padding: 0 20px;
      }
    }
  </style>
  
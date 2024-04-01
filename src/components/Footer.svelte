<!-- Footer.svelte -->

<script>
    export let email = "omidshome@gmail.com";
    export let phoneNumber = "09372282348";
    export let attributionText = "Website created by Omid Abdi";
  </script>
  
  <footer class="footer">
    <div class="content">
      <div class="contact-info">
        <p>Email: <a href="mailto:{email}">{email}</a></p>
        <p>Phone/WhatsApp/Telegram: <a href="tel:{phoneNumber}">{phoneNumber}</a></p>
      </div>
      <div class="attribution">
        <p>{attributionText}</p>
      </div>
    </div>
  </footer>
  
  <style>
    .footer {
      background-color: #333; /* Dark background color */
      color: #fff; /* White text color */
      padding: 20px;
      text-align: center;
    }
  
    .content {
      max-width: 800px;
      margin: 0 auto;
    }
  
    .contact-info {
      margin-bottom: 20px;
    }
  
    .contact-info p {
      margin: 5px 0;
    }
  
    .attribution p {
      font-size: 0.8em; /* Reduced font size for attribution text */
    }

    a{
      color: beige;
      filter: drop-shadow(0 0 5px White);
    }
  </style>
  
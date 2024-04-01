<!-- Rules.svelte -->

<script>
    export let rules = [
      {
        farsi: "قوانین",
        english: "Rules",
        french: "Règles"
      },
      {
        farsi: "۱. دانش‌آموزان می بایست هزینه 10 جلسه را از پیش پرداخت کنند.",
        english: "1. Students must pay for a package of 10 sessions upfront at the beginning of the class.",
        french: "1. Les étudiants doivent payer un forfait de 10 sessions à l'avance au début du cours."
      },
      {
        farsi: "۲. دانش‌آموزان می‌توانند حداکثر ۲ جلسه از بسته 10 جلسه حضور نداشته باشند. جلسه اضافه ارائه نخواهد شد یا جایگزین خواهد شد.",
        english: "2. Students are allowed to be absent for up to 2 sessions out of the 10-session package. Any additional absences will not be refunded or made up.",
        french: "2. Les étudiants sont autorisés à être absents pour un maximum de 2 sessions sur le forfait de 10 sessions. Toute absence supplémentaire ne sera ni remboursée ni rattrapée."
      },
      {
        farsi: "۳. اگر یک دانش‌آموز بیش از ۲ بار در 10 جلسه حضور نداشته باشد، هیچ پولی برگشت داده نخواهد شد یا کلاس جبرانی ارائه نخواهد شد.",
        english: "3. If a student is absent more than 2 times within the 10-session package, there will be no refund or make-up classes provided.",
        french: "3. Si un étudiant est absent plus de 2 fois dans le forfait de 10 sessions, aucun remboursement ou rattrapage ne sera effectué."
      },
      {
        farsi: "۴. دانش‌آموزان باید در زمان دقیق برنامه‌ریزی شده برای درس‌هایشان حاضر باشند. در صورت تأخیر دانش‌آموز، زمان از دوره کلاسش کسر خواهد شد.",
        english: "4. Students must be present at the exact scheduled time for their lessons. If a student is late, the missed time will be deducted from their class duration.",
        french: "4. Les étudiants doivent être présents à l'heure exacte prévue pour leurs leçons. En cas de retard, le temps manqué sera déduit de la durée de leur cours."
      },
      {
        farsi: "۵. اگر یک دانش‌آموز نیاز به لغو کلاس دارد، باید حداقل ۲۴ ساعت قبل به من اطلاع دهد. عدم اطلاع به موقع منجر به حساب شدن جلسه به عنوان حضور نخواهد شد.",
        english: "5. If a student needs to cancel a class, they must notify me at least 24 hours in advance. Failure to do so will result in the session being counted as an absence.",
        french: "5. Si un étudiant a besoin d'annuler un cours, il doit m'en informer au moins 24 heures à l'avance. Le défaut de le faire entraînera le comptage de la session comme une absence."
      },
      {
        farsi: "۶. تعیین زمان برگزاری کلاس‌ها بستگی به موجودیت دارد و باید حداقل ۲۴ ساعت قبل از آن ترتیب داده شود.",
        english: "6. Rescheduling of classes is subject to availability and must be arranged at least 24 hours in advance.",
        french: "6. La reprogrammation des cours est soumise à la disponibilité et doit être organisée au moins 24 heures à l'avance."
      },
      {
        farsi: "۷. ارائه کلاس‌های جبرانی ممکن است با توجه به موجودیت و دلیل حضور نیاز باشد.",
        english: "7. Make-up classes may be provided at the tutor's discretion, depending on availability and the reason for the absence.",
        french: "7. Des cours de rattrapage peuvent être proposés à la discrétion du tuteur, en fonction de la disponibilité et de la raison de l'absence."
      }
    ];
  </script>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300..900;1,300..900&display=swap" rel="stylesheet">
  
  <section class="rules">
    {#each rules as rule}
      <div class="rule">
        <h3 class="title">{rule.farsi}</h3>
        <p class="english">{rule.english}</p>
        <p class="french">{rule.french}</p>
      </div>
    {/each}
  </section>
  
  <style>
    .rules {
      padding: 20px;
      text-align: left;
      background-color: #004080
    }
  
    .rule {
      margin-bottom: 30px;
      border-bottom: 1px solid #ccc;
      padding-bottom: 20px;
    }
  
    .title {
      font-size: 1.2em;
      font-weight: bold;
      font-family:Rubik ;
      margin-bottom: 10px;
      direction: rtl; /* Right-to-left direction for Farsi */
    }
  
    .english, .french {
      margin-bottom: 10px;
      direction: ltr; /* Left-to-right direction for English and French */
    }
  
    /* Responsive styles */
    @media (max-width: 768px) {
      .title {
        font-size: 1em;
      }
  
      .english, .french {
        font-size: 0.9em;
      }
    }
  </style>
  
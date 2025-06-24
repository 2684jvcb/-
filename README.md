<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>مدرسة خلفاء التعليمية</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="manifest" href="manifest.json">
  <meta name="theme-color" content="#d4af37">
  <style>
    body {
      background-color: #1e1e1e;
      color: #d4af37;
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.8;
    }
    header {
      background: linear-gradient(to right, #6a5200, #bfa235);
      text-align: center;
      padding: 30px 15px;
    }
    header h1 {
      margin: 0;
      font-size: 2.5em;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      color: #fff8dc;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      color: #ffd700;
    }
    main {
      padding: 30px 20px;
      max-width: 900px;
      margin: auto;
    }
    section {
      background: #2c2c2c;
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 0 10px #d4af37;
      margin-bottom: 30px;
    }
    h2 {
      border-bottom: 2px solid #d4af37;
      padding-bottom: 10px;
      margin-bottom: 20px;
    }
    footer {
      background: #333;
      color: #f5deb3;
      text-align: center;
      padding: 20px;
    }
    .contact-link {
      color: #ffd700;
      font-weight: bold;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>مدرسة خلفاء التعليمية</h1>
    <nav>
      <a href="#about">عن المدرسة</a>
      <a href="#mission">رسالتنا</a>
      <a href="#departments">الأقسام</a>
      <a href="#faq">الأسئلة</a>
      <a href="#contact">تواصل</a>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>عن المدرسة</h2>
      <p>
        مدرسة خلفاء التعليمية مؤسسة علمية روحية، متخصصة في تعليم العلوم الربانية والنورانية،
        وتُعنى بالكشف والتصدي للسحر والشياطين، عبر مناهج روحية مستندة إلى الحكمة القديمة والعلم اللدني.
      </p>
    </section>

    <section id="mission">
      <h2>رسالتنا وأهدافنا</h2>
      <ul>
        <li>نشر العلم النوراني وعلوم الفتح الرباني.</li>
        <li>تحصين النفس والروح من المؤثرات السحرية والشيطانية.</li>
        <li>إعداد جيل خلفاء مؤمن بالله، عالم بأسرار الحماية والطاقة النورانية.</li>
        <li>ربط الإنسان بالعلوم اللدنية والأسرار المخفية للحكمة الإلهية.</li>
      </ul>
    </section>

    <section id="departments">
      <h2>الأقسام التعليمية</h2>
      <ul>
        <li>📖 قسم العلوم الروحية (الكشف، الطاقات، النورانية)</li>
        <li>🛡️ قسم الحرب على السحر والشياطين</li>
        <li>⚔️ قسم استخدام السيوف الذهبية والرموز</li>
        <li>📜 قسم الدروس النظرية والعملية</li>
      </ul>
    </section>

    <section id="faq">
      <h2>أسئلة متكررة</h2>
      <p><strong>هل الدروس مجانية؟</strong><br>نعم، معظم دروس المدرسة متاحة مجاناً لمن يبحث عن العلم الصادق.</p>
      <p><strong>هل هناك شهادات أو دورات؟</strong><br>نعم، نوفر دورات وشهادات رقمية للمتعلمين المنتظمين.</p>
      <p><strong>كيف أحصل على جلسة كشف روحاني؟</strong><br>بالتواصل معنا عبر الرقم الرسمي أو الواتساب.</p>
    </section>

    <section id="contact">
      <h2>تواصل معنا</h2>
      <p>للاستفسار والحجز، يرجى التواصل على:</p>
      <p>📞 <strong>+967 776111179</strong></p>
      <p>📱 <a href="https://wa.me/967776111179" class="contact-link">راسلنا على الواتساب</a></p>
    </section>
  </main>

  <footer>
    © 2025 مدرسة خلفاء التعليمية — جميع الحقوق محفوظة
  </footer>

  <script>
    if ('serviceWorker' in navigator) {
      navigator.serviceWorker.register('/sw.js')
        .then(() => console.log('تم تسجيل الـ Service Worker'));
    }
  </script>
</body>
</html>

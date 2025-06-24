# -
العلوم النروانيه العلياء وعلوم حرب وقتال السحره والشياطين بعلم الكتاب 
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>مدرسة خلفاء التعليمية</title>
    <link rel="manifest" href="manifest.json" />
    <meta name="theme-color" content="#d4af37" />
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background: #1e1e1e;
            color: #d4af37; /* ذهبي */
            margin: 0;
            padding: 0;
        }
        header {
            background: linear-gradient(90deg, #bfa235, #6a5200);
            padding: 20px;
            text-align: center;
            position: relative;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
            letter-spacing: 3px;
            font-weight: bold;
        }
        .logo {
            position: absolute;
            left: 20px;
            top: 15px;
            width: 60px;
            height: 60px;
        }
        nav {
            margin-top: 10px;
        }
        nav a {
            color: #f5deb3;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1em;
        }
        nav a:hover {
            color: #ffd700;
            text-shadow: 0 0 5px #ffd700;
        }
        main {
            padding: 30px 20px;
            max-width: 900px;
            margin: auto;
        }
        section {
            margin-bottom: 40px;
            background: #2c2c2c;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 0 15px #bfa235;
        }
        h2 {
            color: #ffd700;
            margin-bottom: 15px;
            border-bottom: 2px solid #d4af37;
            padding-bottom: 8px;
        }
        footer {
            background: #6a5200;
            color: #f5deb3;
            text-align: center;
            padding: 15px;
            margin-top: 50px;
            font-size: 0.9em;
        }
        .contact-info {
            font-size: 1.2em;
            margin-top: 10px;
        }
        a.contact-link {
            color: #ffd700;
            text-decoration: none;
            font-weight: bold;
        }
        a.contact-link:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <img src="logo.png" alt="شعار المدرسة" class="logo" />
        <h1>مدرسة خلفاء التعليمية</h1>
        <nav>
            <a href="#about">عن المدرسة</a>
            <a href="#services">خدماتنا</a>
            <a href="#contact">تواصل معنا</a>
        </nav>
    </header>
    <main>
        <section id="about">
            <h2>عن المدرسة</h2>
            <p>مدرسة خلفاء التعليمية متخصصة في العلوم الربانية والنورانية، مع تركيز خاص على تعليم فنون حرب وقتال السحرة والشياطين.</p>
        </section>
        <section id="services">
            <h2>خدماتنا</h2>
            <ul>
                <li>دروس وورش تعليمية في العلوم الروحية.</li>
                <li>تعليم استخدام رموز السيوف الذهبية والعلم اللدني.</li>
                <li>جلسات تدريبية على الدفاع الروحي.</li>
                <li>دعم وتواصل مباشر عبر الهاتف والواتساب.</li>
            </ul>
        </section>
        <section id="contact">
            <h2>تواصل معنا</h2>
            <p>للاستفسار والحجز، يرجى الاتصال على الرقم التالي:</p>
            <p class="contact-info">+967 776111179</p>
            <p>أو عبر الواتساب: <a href="https://wa.me/967776111179" class="contact-link" target="_blank" rel="noopener noreferrer">اضغط هنا للتواصل</a></p>
        </section>
    </main>
    <footer>
        جميع الحقوق محفوظة © 2025 مدرسة خلفاء التعليمية
    </footer>

    <script>
      if ('serviceWorker' in navigator) {
        navigator.serviceWorker.register('/sw.js')
          .then(() => console.log('Service Worker Registered'));
      }
    </script>
</body>
</html>

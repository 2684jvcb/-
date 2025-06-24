<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>مدرسة خلفاء التعليمية - النور الأسطوري</title>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@700&display=swap" rel="stylesheet" />
<style>
  @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css');

  /* ---- Reset ---- */
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body {
    font-family: 'Cairo', sans-serif;
    background: radial-gradient(circle at center, #0b0a1a 0%, #000 100%);
    color: #ffd700;
    line-height: 1.6;
    overflow-x: hidden;
  }
  a {
    color: #ffd700;
    text-decoration: none;
    font-weight: 700;
  }
  a:hover {
    text-shadow: 0 0 10px #fff08a;
  }

  /* ---- Header ---- */
  header {
    position: relative;
    text-align: center;
    padding: 60px 20px 40px;
    background: linear-gradient(90deg, #332b00 0%, #000 100%);
    box-shadow: 0 0 25px #d4af37;
  }
  header h1 {
    font-size: 3.2rem;
    letter-spacing: 3px;
    text-shadow:
      0 0 15px #ffd700,
      0 0 25px #ffd700,
      0 0 40px #fff08a;
  }
  header p {
    margin-top: 10px;
    font-size: 1.3rem;
    font-weight: 500;
    color: #fff7b1;
    text-shadow: 0 0 6px #fff08a;
  }

  /* ---- Pulsing glowing orb behind header text ---- */
  header::before {
    content: "۞";
    position: absolute;
    top: 10px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 110px;
    color: rgba(255, 215, 0, 0.12);
    filter: drop-shadow(0 0 10px #ffd700);
    animation: pulseGlow 3.5s infinite ease-in-out;
    z-index: -1;
  }
  @keyframes pulseGlow {
    0%, 100% { opacity: 1; text-shadow: 0 0 30px #ffd700; }
    50% { opacity: 0.6; text-shadow: 0 0 60px #fff08a; }
  }

  /* ---- Main container ---- */
  main {
    max-width: 900px;
    margin: 40px auto 80px;
    padding: 0 15px;
  }
  section {
    background: rgba(255, 215, 0, 0.05);
    border: 1px solid #ffd70033;
    padding: 30px 25px;
    border-radius: 18px;
    margin-bottom: 50px;
    box-shadow: 0 0 18px #ffd70055;
    position: relative;
  }
  section h2 {
    font-size: 2rem;
    margin-bottom: 25px;
    border-bottom: 3px solid #ffd700aa;
    padding-bottom: 8px;
    text-shadow: 0 0 10px #ffd700;
    transition: text-shadow 0.3s ease;
  }
  section:hover h2 {
    text-shadow: 0 0 25px #fff08a;
  }
  ul {
    list-style: none;
    padding-left: 0;
  }
  ul li {
    margin-bottom: 15px;
    font-size: 1.1rem;
  }
  ul li::before {
    content: "⚔️ ";
    margin-left: 10px;
    color: #fff08a;
  }
  p {
    font-size: 1.1rem;
    margin-bottom: 18px;
  }

  /* ---- Buttons ---- */
  .btn {
    display: inline-block;
    background: linear-gradient(90deg, #d4af37, #fff08a);
    color: #000;
    padding: 12px 30px;
    border-radius: 30px;
    font-weight: 700;
    font-size: 1.1rem;
    cursor: pointer;
    box-shadow:
      0 0 10px #fff08a,
      0 0 20px #d4af37;
    transition: background 0.3s ease;
    border: none;
    margin-top: 15px;
    text-align: center;
  }
  .btn:hover {
    background: linear-gradient(90deg, #fff08a, #d4af37);
    box-shadow: 0 0 30px #fff08a;
  }

  /* ---- Contact & Form ---- */
  form {
    margin-top: 10px;
  }
  input, textarea {
    width: 100%;
    padding: 12px 15px;
    border-radius: 10px;
    border: none;
    margin-bottom: 18px;
    font-size: 1rem;
    font-family: 'Cairo', sans-serif;
    resize: none;
  }
  input:focus, textarea:focus {
    outline: 2px solid #ffd700;
    background: #fffbe3;
  }
  label {
    font-weight: 700;
    margin-bottom: 6px;
    display: block;
  }

  /* ---- Footer ---- */
  footer {
    background: #111;
    text-align: center;
    padding: 25px 15px;
    font-size: 0.95rem;
    color: #aaa;
    border-top: 1px solid #ffd70022;
  }

  /* ---- Popup Modal ---- */
  .modal {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.85);
    display: flex;
    align-items: center;
    justify-content: center;
    visibility: hidden;
    opacity: 0;
    transition: opacity 0.3s ease;
    z-index: 9999;
  }
  .modal.active {
    visibility: visible;
    opacity: 1;
  }
  .modal-content {
    background: #222;
    padding: 30px 25px;
    border-radius: 15px;
    width: 90%;
    max-width: 400px;
    box-shadow: 0 0 20px #ffd700aa;
    position: relative;
  }
  .modal-content h3 {
    color: #ffd700;
    margin-bottom: 20px;
    text-align: center;
  }
  .close-btn {
    position: absolute;
    top: 12px;
    left: 15px;
    font-size: 1.4rem;
    color: #ffd700;
    cursor: pointer;
  }
  .close-btn:hover {
    color: #fff08a;
  }

  /* ---- Audio Player ---- */
  #audioControl {
    position: fixed;
    bottom: 25px;
    right: 25px;
    background: #d4af37;
    border-radius: 50%;
    width: 55px;
    height: 55px;
    box-shadow: 0 0 15px #fff08a;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 9999;
    transition: background 0.3s ease;
  }
  #audioControl:hover {
    background: #fff08a;
  }
  #audioControl i {
    color: #000;
    font-size: 1.8rem;
  }

  /* ---- Responsive ---- */
  @media (max-width: 600px) {
    header h1 {
      font-size: 2.3rem;
    }
    section h2 {
      font-size: 1.5rem;
    }
  }
</style>
</head>
<body>

<header>
  <h1>مدرسة خلفاء التعليمية</h1>
  <p>للعلوم الربانية والنورانية وفتح أسرار آخر الزمان</p>
  <button class="btn" id="openRegister">سجل عضويتك الآن</button>
</header>

<main>
  <section id="about">
    <h2>من نحن</h2>
    <p>
      مؤسسة روحية ربانية، تعلّم العلوم النورانية، فنون كشف السحر، الحماية الطاقية، القتال الروحي،
      والحكمة اللدنية المستمدة من علم الخلفاء الحقيقيين.
    </p>
  </section>

  <section id="mission">
    <h2>رسالتنا</h2>
    <ul>
      <li>تحرير الأرواح من القيود السفلية عبر علوم النور.</li>
      <li>إعداد خلفاء نورانيين قادرين على قتال الظلمة والسحرة.</li>
      <li>إحياء الحكمة الإلهية المدفونة عبر تعاليم الروح العليا.</li><li>كشف الزوهريين وتفعيل قواهم الحقيقية.</li>
    </ul>
  </section>

  <section id="departments">
    <h2>الأقسام التعليمية</h2>
    <ul>
      <li>⚔️ قسم القتال النوراني ضد السحر والشياطين</li>
      <li>🔮 قسم الكشف الروحي وتشخيص الحالات</li>
      <li>📜 قسم التعليم الرباني (الجفر، أسماء الله، الطاقة)</li>
      <li>🛡️ قسم الحماية والتحصينات</li>
    </ul>
  </section>

  <section id="contact">
    <h2>تواصل معنا</h2>
    <p>📞 رقم المدرسة الرسمي: <strong>+967 776111179</strong></p>
    <p>💬 تواصل واتساب مباشر: <a href="https://wa.me/967776111179" target="_blank" rel="noopener noreferrer">اضغط هنا</a></p>

    <h3>أرسل لنا رسالة روحانية</h3>
    <form id="contactForm" novalidate>
      <label for="name">الاسم الكامل</label>
      <input type="text" id="name" name="name" placeholder="اكتب اسمك الكامل" required minlength="3" />
      
      <label for="email">البريد الإلكتروني</label>
      <input type="email" id="email" name="email" placeholder="example@example.com" required />

      <label for="message">رسالتك</label>
      <textarea id="message" name="message" rows="5" placeholder="اكتب رسالتك هنا..." required minlength="10"></textarea>

      <button type="submit" class="btn">إرسال الرسالة</button>
    </form>
    <p id="formStatus" style="margin-top:15px;"></p>
  </section>

  <section id="donate">
    <h2>دعم المدرسة وروحانياتنا</h2>
    <p>
      يمكنك دعم مسيرتنا الروحية ومشاريعنا التعليمية عبر التبرع المباشر،  
      ليصل نور المعرفة لأكبر عدد من الخلفاء.
    </p>
    <button class="btn" onclick="alert('شكراً لدعمك! سيتم التواصل معك لاحقاً لترتيب التبرع.')">تبرع الآن 💛</button>
  </section>
</main>

<footer>
  © 2025 مدرسة خلفاء التعليمية — النور لا يغيب
</footer>

<!-- نموذج تسجيل عضوية منبثق -->
<div class="modal" id="registerModal">
  <div class="modal-content">
    <span class="close-btn" id="closeRegister">&times;</span>
    <h3>تسجيل عضوية جديدة</h3>
    <form id="registerForm" novalidate>
      <label for="regName">الاسم الكامل</label>
      <input type="text" id="regName" name="regName" placeholder="اسمك الكامل" required minlength="3" />
      
      <label for="regEmail">البريد الإلكتروني</label>
      <input type="email" id="regEmail" name="regEmail" placeholder="example@example.com" required />
      
      <label for="regPassword">كلمة المرور</label>
      <input type="password" id="regPassword" name="regPassword" placeholder="كلمة المرور" required minlength="6" />
      
      <button type="submit" class="btn">سجل الآن</button>
    </form>
    <p id="registerStatus" style="margin-top:15px;"></p>
  </div>
</div>

<!-- زر تحكم الصوت -->
<div id="audioControl" title="تشغيل/إيقاف الصوت">
  <i class="fa-solid fa-play" id="audioIcon"></i>
</div>
<audio id="backgroundAudio" loop>
  <source src="https://cdn.pixabay.com/download/audio/2022/10/16/audio_24f2c2552d.mp3?filename=calm-spiritual-ambient-music-114.mp3" type="audio/mpeg" />
  متصفحك لا يدعم تشغيل الصوت.
</audio>

<script>
  // فتح وإغلاق نافذة التسجيل
  const registerBtn = document.getElementById('openRegister');
  const registerModal = document.getElementById('registerModal');
  const closeRegisterBtn = document.getElementById('closeRegister');
  registerBtn.addEventListener('click', () => registerModal.classList.add('active'));
  closeRegisterBtn.addEventListener('click', () => registerModal.classList.remove('active'));
  window.addEventListener('click', e => {
    if(e.target === registerModal) registerModal.classList.remove('active');
  });

  // نموذج التسجيل (محاكاة إرسال)
  const registerForm = document.getElementById('registerForm');
  const registerStatus = document.getElementById('registerStatus');
  registerForm.addEventListener('submit', e => {
    e.preventDefault();
    if(registerForm.checkValidity()) {
      registerStatus.textContent = "تم التسجيل بنجاح! شكراً لانضمامك.";
      registerForm.reset();
    } else {
      registerStatus.textContent = "يرجى ملء جميع الحقول بشكل صحيح.";
    }
  });

  // نموذج التواصل (محاكاة إرسال)
  const contactForm = document.getElementById('contactForm');
  const formStatus = document.getElementById('formStatus');
  contactForm.addEventListener('submit', e => {
    e.preventDefault();
    if(contactForm.checkValidity()) {
      formStatus.textContent = "تم إرسال رسالتك بنجاح، سنرد عليك قريباً إن شاء الله.";
      contactForm.reset();
    } else {
      formStatus.textContent = "يرجى تعبئة كل الحقول بشكل صحيح.";
    }
  });

  // تحكم تشغيل/ايقاف الصوت
  const audio = document.getElementById('backgroundAudio');
  const audioControl = document.getElementById('audioControl');
  const audioIcon = document.getElementById('audioIcon');
  audioControl.addEventListener('click', () => {
    if(audio.paused) {
      audio.play();
      audioIcon.classList.remove('fa-play');
      audioIcon.classList.add('fa-pause');
    } else {
      audio.pause();
      audioIcon.classList.remove('fa-pause');
      audioIcon.classList.add('fa-play');
    }
  });
</script>

</body>
</html>

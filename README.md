<a class="btn btn-primary"
   href="https://www.facebook.com/"
   target="_blank" rel="noopener noreferrer">
  زُر فيسبوك ↗
</a>
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#080d18">
  <meta name="description" content="HM18 - حكيم، مصور وصانع محتوى إبداعي من زيامة منصورية، الجزائر.">
  <title>HM18 | حكيم - صانع محتوى بصري</title>

  <style>
    :root {
      --bg: #080d18;
      --panel: #101a2b;
      --blue: #39cfff;
      --text: #f3f7ff;
      --muted: #9baec5;
      --border: rgba(57, 207, 255, .18);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Tahoma, Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.8;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    button {
      font: inherit;
    }

    .sidebar {
      width: 255px;
      height: 100vh;
      position: fixed;
      top: 0;
      right: 0;
      z-index: 100;
      background: #0c1423;
      border-left: 1px solid var(--border);
      padding: 32px 22px;
      display: flex;
      flex-direction: column;
    }

    .logo {
      font-size: 38px;
      font-weight: 900;
      letter-spacing: 3px;
      color: var(--blue);
      text-shadow: 0 0 22px rgba(57, 207, 255, .5);
      text-align: center;
    }

    .logo-sub {
      text-align: center;
      color: var(--muted);
      font-size: 12px;
      margin-bottom: 45px;
    }

    .nav-title {
      color: #71869f;
      font-size: 12px;
      margin-bottom: 12px;
    }

    .nav-links {
      display: flex;
      flex-direction: column;
      gap: 10px;
    }

    .nav-links a {
      padding: 12px 15px;
      border-radius: 10px;
      color: #c1cee0;
      transition: .25s;
    }

    .nav-links a:hover,
    .nav-links a.active {
      background: rgba(57, 207, 255, .1);
      color: var(--blue);
      box-shadow: inset -3px 0 var(--blue);
    }

    .sidebar-bottom {
      margin-top: auto;
      text-align: center;
      color: #7588a0;
      font-size: 12px;
    }

    .main {
      margin-right: 255px;
      overflow: hidden;
    }

    .hero {
      min-height: 90vh;
      padding: 90px 7%;
      display: flex;
      align-items: center;
      background:
        radial-gradient(ellipse at 80% 25%, rgba(0, 147, 210, .16), transparent 45%),
        linear-gradient(135deg, #080d18, #101c30);
      position: relative;
    }

    .hero-content {
      max-width: 750px;
    }

    .eyebrow {
      display: inline-block;
      padding: 7px 15px;
      border: 1px solid var(--border);
      border-radius: 30px;
      color: var(--blue);
      background: rgba(57, 207, 255, .06);
      margin-bottom: 24px;
      font-size: 14px;
    }

    .hero h1 {
      font-size: clamp(38px, 6vw, 68px);
      line-height: 1.3;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: var(--blue);
      text-shadow: 0 0 28px rgba(57, 207, 255, .18);
    }

    .hero p {
      color: var(--muted);
      font-size: 17px;
      max-width: 600px;
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 13px;
    }

    .btn {
      display: inline-block;
      padding: 12px 24px;
      border-radius: 10px;
      border: 1px solid var(--blue);
      transition: .25s;
      cursor: pointer;
    }

    .btn-primary {
      background: var(--blue);
      color: #07111e;
      font-weight: bold;
    }

    .btn-outline {
      color: var(--blue);
      background: transparent;
    }

    .btn:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 25px rgba(57, 207, 255, .14);
    }

    .hero-mark {
      position: absolute;
      left: 5%;
      bottom: 35px;
      color: rgba(57, 207, 255, .07);
      font-size: clamp(65px, 12vw, 150px);
      font-weight: 900;
      pointer-events: none;
    }

    section.content-section {
      padding: 85px 7%;
      scroll-margin-top: 20px;
    }

    .section-heading {
      margin-bottom: 35px;
    }

    .section-heading small {
      color: var(--blue);
      font-size: 13px;
    }

    .section-heading h2 {
      font-size: clamp(27px, 4vw, 38px);
      margin-top: 5px;
    }

    .section-heading p {
      color: var(--muted);
      margin-top: 10px;
    }

    .about-box {
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 30px;
    }

    .about-box p {
      color: #b5c5d9;
      margin-bottom: 12px;
    }

    .tag-list {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 22px;
    }

    .tag {
      padding: 7px 13px;
      border-radius: 8px;
      background: rgba(57, 207, 255, .08);
      border: 1px solid var(--border);
      color: var(--blue);
      font-size: 13px;
    }

    .work-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 20px;
    }

    .work-card {
      min-height: 210px;
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 26px;
      background:
        radial-gradient(circle at 90% 10%, rgba(57, 207, 255, .1), transparent 55%),
        var(--panel);
      transition: .3s;
    }

    .work-card:hover {
      transform: translateY(-5px);
      border-color: var(--blue);
    }

    .work-icon {
      font-size: 30px;
      margin-bottom: 13px;
    }

    .work-card h3 {
      margin-bottom: 8px;
      color: var(--text);
    }

    .work-card p {
      color: var(--muted);
      font-size: 14px;
    }

    .empty-note {
      margin-top: 20px;
      color: #8195ad;
      font-size: 13px;
    }

    .contact-box {
      background: var(--panel);
      border: 1px solid var(--border);
      border-radius: 18px;
      padding: 30px;
    }

    .contact-box p {
      color: var(--muted);
      margin-bottom: 22px;
    }

    footer {
      padding: 25px 7%;
      border-top: 1px solid var(--border);
      color: #8497ad;
      font-size: 13px;
      text-align: center;
    }

    .menu-toggle {
      display: none;
      position: fixed;
      top: 15px;
      right: 15px;
      z-index: 200;
      width: 45px;
      height: 45px;
      background: var(--panel);
      border: 1px solid var(--border);
      color: var(--blue);
      border-radius: 10px;
      font-size: 23px;
      cursor: pointer;
    }

    .overlay {
      display: none;
    }

    @media (max-width: 850px) {
      .sidebar {
        transform: translateX(100%);
        transition: transform .3s ease;
        width: 260px;
      }

      .sidebar.open {
        transform: translateX(0);
      }

      .main {
        margin-right: 0;
      }

      .menu-toggle {
        display: block;
      }

      .overlay.show {
        display: block;
        position: fixed;
        inset: 0;
        background: rgba(0, 0, 0, .6);
        z-index: 90;
      }

      .hero {
        min-height: 82vh;
        padding: 100px 7% 70px;
      }

      section.content-section {
        padding: 65px 6%;
      }
    }

    @media (max-width: 520px) {
      .work-grid {
        grid-template-columns: 1fr;
      }

      .hero h1 {
        font-size: 38px;
      }

      .hero p {
        font-size: 15px;
      }

      .about-box,
      .contact-box {
        padding: 22px;
      }
    }
  </style>
</head>

<body>

  <button class="menu-toggle" id="menuToggle"
          aria-label="فتح القائمة" aria-expanded="false"
          aria-controls="sidebar">☰</button>

  <div class="overlay" id="overlay"></div>

  <aside class="sidebar" id="sidebar">
    <div class="logo">HM18</div>
    <div class="logo-sub">الإبداع يبدأ من هنا</div>

    <div class="nav-title">القائمة الرئيسية</div>

    <nav class="nav-links">
      <a href="#home" class="active">⌂ &nbsp; الرئيسية</a>
      <a href="#about">◈ &nbsp; من أنا</a>
      <a href="#portfolio">▦ &nbsp; معرض الأعمال</a>
      <a href="#contact">✉ &nbsp; اتصل بي</a>
    </nav>

    <div class="sidebar-bottom">
      <p>صورة تحكي قصة</p>
      <p>© 2026 HM18</p>
    </div>
  </aside>

  <main class="main">

    <header class="hero" id="home">
      <div class="hero-content">
        <span class="eyebrow">📸 تصوير فوتوغرافي وصناعة المحتوى</span>

        <h1>
          مرحبًا بكم في عالم<br>
          <span>HM18 الإبداعي</span>
        </h1>

        <p>
          معكم حكيم، صانع محتوى بصري من زيامة منصورية،
          الجزائر. أشارككم شغفي بالتصوير، جمال الطبيعة،
          والمشاهد التي تستحق أن تبقى في الذاكرة.
        </p>

        <div class="buttons">
          <a href="#portfolio" class="btn btn-primary">اكتشف أعمالي ←</a>
          <a href="#about" class="btn btn-outline">تعرّف عليّ</a>
        </div>
      </div>

      <div class="hero-mark">HM18</div>
    </header>

    <section class="content-section" id="about">
      <div class="section-heading">
        <small>01 — من أنا</small>
        <h2>وراء كل صورة حكاية</h2>
        <p>شغف بالصورة، واهتمام بالتفاصيل.</p>
      </div>

      <div class="about-box">
        <p>
          أنا حكيم، مصوّر وصانع محتوى بصري من زيامة منصورية،
          ولاية جيجل، الجزائر.
        </p>
        <p>
          أؤمن أن الصورة ليست مجرد لقطة، بل وسيلة لنقل
          الإحساس وإبراز جمال الأماكن والناس والحياة اليومية.
        </p>
        <p>
          من المناظر الطبيعية إلى الجسور والمعالم،
          أسعى دائمًا إلى تقديم محتوى إبداعي يجمع بين
          البساطة والجمال والتكنولوجيا.
        </p>

        <div class="tag-list">
          <span class="tag">التصوير الفوتوغرافي</span>
          <span class="tag">صناعة المحتوى</span>
          <span class="tag">الفيديو الإبداعي</span>
          <span class="tag">الذكاء الاصطناعي</span>
        </div>
      </div>
    </section>

    <section class="content-section" id="portfolio">
      <div class="section-heading">
        <small>02 — معرض الأعمال</small>
        <h2>اكتشف عالم صوري</h2>
        <p>مساحات من الإبداع تنتظر عرض أفضل أعمالي.</p>
      </div>

      <div class="work-grid">
        <article class="work-card">
          <div class="work-icon">🌊</div>
          <h3>جمال الطبيعة</h3>
          <p>البحر، الجبال، الغروب والمناظر الطبيعية الجزائرية.</p>
        </article>

        <article class="work-card">
          <div class="work-icon">🌉</div>
          <h3>المعالم والمدن</h3>
          <p>اكتشاف المدن والمعالم المعمارية واللقطات المميزة.</p>
        </article>

        <article class="work-card">
          <div class="work-icon">🎬</div>
          <h3>الفيديو الإبداعي</h3>
          <p>مشاهد بصرية وحركة سينمائية تحوّل اللحظات إلى قصص.</p>
        </article>

        <article class="work-card">
          <div class="work-icon">✨</div>
          <h3>الإبداع بالذكاء الاصطناعي</h3>
          <p>أفكار بصرية وتجارب إبداعية تجمع التصوير بالتكنولوجيا.</p>
        </article>
      </div>

      <p class="empty-note">
        ملاحظة: هذه بطاقات تعريفية مؤقتة. نقدروا نضيفوا
        صورك الحقيقية وروابط فيديوهاتك في الخطوة القادمة.
      </p>
    </section>

    <section class="content-section" id="contact">
      <div class="section-heading">
        <small>03 — التواصل</small>
        <h2>خلّينا نتواصلوا</h2>
        <p>عندك مشروع أو فكرة إبداعية؟ مرحبًا بك.</p>
      </div>

      <div class="contact-box">
        <h3>HM18 — حكيم</h3>
        <p>
          للتعاون والمشاريع والاستفسارات، تقدر تتواصل
          معي عبر صفحتي على مواقع التواصل الاجتماعي.
        </p>

        <!-- أضف رابط صفحتك الحقيقي مكان الرابط التالي -->
        <a class="btn btn-primary"
           href="https://www.facebook.com/"
           target="_blank" rel="noopener noreferrer">
          زُر فيسبوك ↗
        </a>
      </div>
    </section>

    <footer>
      <p>© 2026 HM18 — جميع الحقوق محفوظة</p>
      <p>صُنع بشغف في الجزائر 🇩🇿</p>
    </footer>

  </main>

  <script>
    const toggle = document.getElementById('menuToggle');
    const sidebar = document.getElementById('sidebar');
    const overlay = document.getElementById('overlay');
    const links = document.querySelectorAll('.nav-links a');

    function closeMenu() {
      sidebar.classList.remove('open');
      overlay.classList.remove('show');
      toggle.setAttribute('aria-expanded', 'false');
      toggle.textContent = '☰';
    }

    toggle.addEventListener('click', function () {
      const isOpen = sidebar.classList.toggle('open');
      overlay.classList.toggle('show', isOpen);
      toggle.setAttribute('aria-expanded', String(isOpen));
      toggle.textContent = isOpen ? '✕' : '☰';
    });

    overlay.addEventListener('click', closeMenu);

    links.forEach(function (link) {
      link.addEventListener('click', function () {
        links.forEach(function (item) {
          item.classList.remove('active');
        });
        link.classList.add('active');
        closeMenu();
      });
    });
  </script>

</body>
</html>
# hm18-portfolio
موقع H-M-18 الرسمي لصناعة الفيديوهات السينمائية بالذكاء الاصطناعي وتحويل الصور إلى مشاهد متحركة.

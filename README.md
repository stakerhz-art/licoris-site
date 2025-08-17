<!doctype html>
<html lang="ru" data-theme="dark">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>ЛИКОРИС — Minecraft сервер</title>
  <meta name="description" content="Официальный сайт Minecraft-сервера ЛИКОРИС: IP, донат, поддержка." />
  <style>
    :root {
      --bg: #0a0a0a;
      --panel: #111;
      --panel-2: #1a1a1a;
      --text: #f5f5f5;
      --muted: #b3b3b3;
      --accent: #ff2a2a;
      --accent-2: #cc0000;
      --danger: #ff4d4d;
      --shadow: 0 10px 30px rgba(0,0,0,.5);
      --radius: 16px;
    }

    body {
      margin: 0;
      font: 16px/1.6 system-ui, sans-serif;
      color: var(--text);
      background: var(--bg);
    }
    a { color: inherit; text-decoration: none; }
    .container { max-width: 1100px; margin: 0 auto; padding: 0 20px; }
    .card { background: linear-gradient(180deg, var(--panel), var(--panel-2)); border-radius: var(--radius); box-shadow: var(--shadow); }
    .btn {
      display: inline-flex; align-items: center; gap: 10px; border: 0; padding: 12px 18px; border-radius: 12px; cursor: pointer; font-weight: 700;
      background: linear-gradient(135deg, var(--accent), var(--accent-2)); color: #fff;
      transition: transform .1s ease, filter .2s ease;
    }
    .btn:hover{ transform: translateY(-1px); filter: brightness(1.1); }
    .btn.secondary { background: #222; color: var(--text); }

    header { background: #0d0d0d; border-bottom: 1px solid #222; position: sticky; top: 0; z-index: 30; }
    .nav { display: flex; align-items: center; justify-content: space-between; height: 64px; }
    .brand { display: flex; align-items: center; gap: 12px; font-weight: 900; color: var(--accent); font-size: 20px; }
    .brand img { width: 28px; height: 28px; }
    nav ul { list-style: none; display: flex; gap: 18px; margin: 0; padding: 0; }
    nav a{ opacity: .9; padding: 8px 10px; border-radius: 10px; }
    nav a:hover{ background: #222; }

    .hero { padding: 80px 0; text-align: center; }
    .title { font-size: 44px; font-weight: 900; color: var(--accent); margin: 0 0 12px; }
    .subtitle { color: var(--muted); margin-bottom: 20px; }

    section { padding: 60px 0; }
    section h2 { font-size: 32px; margin: 0 0 18px; text-align:center; color: var(--accent); }
    .grid { display: grid; gap: 20px; }
    .grid.cols-2 { grid-template-columns: repeat(2, 1fr); }

    .donate .card { padding: 20px; text-align: center; }
    .donate h3 { margin: 10px 0; font-size: 20px; color: var(--accent); }

    footer { border-top: 1px solid #222; padding: 28px 0; color: var(--muted); text-align: center; }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="brand">
        <img src="https://cdn-icons-png.flaticon.com/512/337/337946.png" alt="Логотип" />
        ЛИКОРИС
      </div>
      <nav>
        <ul>
          <li><a href="#about">О сервере</a></li>
          <li><a href="#donate">Донат</a></li>
          <li><a href="#support">Поддержка</a></li>
        </ul>
      </nav>
      <a class="btn" href="#join">Играть</a>
    </div>
  </header>

  <main class="hero container">
    <h1 class="title">Minecraft сервер ЛИКОРИС</h1>
    <p class="subtitle">Красный и чёрный мир для настоящих воинов. Версия 1.20+ • PvP, выживание, экономика.</p>
    <button class="btn" id="copyIp">Скопировать IP</button>
    <p class="subtitle">IP: <b id="serverIp">lycoris.cfd</b></p>
  </main>

  <section id="about">
    <div class="container">
      <h2>О сервере</h2>
      <p style="text-align:center; color:var(--muted)">ЛИКОРИС — это честный сервер без привилегий. Донат существует только для поддержки проекта.</p>
    </div>
  </section>

  <section id="donate" class="donate">
    <div class="container">
      <h2>Донат</h2>
      <p style="text-align:center; color:var(--muted)">Поддержи сервер суммой от <b>50₴</b> (или в $ в зависимости от страны). Донат не даёт игровых преимуществ и привилегий.</p>
      <div class="grid cols-2" style="margin-top:30px">
        <div class="card">
          <h3>Поддержка</h3>
          <p class="muted">от 50₴ / 2$</p>
          <p>Вы помогаете оплачивать хостинг и развитие проекта.</p>
          <button class="btn">Задонатить</button>
        </div>
        <div class="card">
          <h3>Поддержка+ благодарность</h3>
          <p class="muted">от 100₴ / 4$</p>
          <p>Ваш ник появится в списке благодарности на сайте.</p>
          <button class="btn">Задонатить</button>
        </div>
      </div>
    </div>
  </section>

  <section id="support">
    <div class="container">
      <h2>Поддержка</h2>
      <p style="text-align:center; color:var(--muted)">Возникли вопросы или проблемы? Свяжитесь с нами через Discord или email.</p>
      <div style="display:flex; gap:10px; justify-content:center; margin-top:20px">
        <a class="btn secondary" href="#">Discord</a>
        <a class="btn secondary" href="mailto:support@licorix.ru">Email</a>
      </div>
    </div>
  </section>

  <section id="join">
    <div class="container">
      <h2>Присоединяйся!</h2>
      <p style="text-align:center; color:var(--muted)">IP: lycoris.cfd • Версия 1.20+</p>
      <div style="text-align:center; margin-top:20px">
        <button class="btn" id="copyIp2">Скопировать IP</button>
      </div>
    </div>
  </section>

  <footer>
    <div class="container">© <span id="year"></span> ЛИКОРИС. Неофициальный сайт Mojang.</div>
  </footer>

  <script>
    const SERVER_IP = 'lycoris.cfd';
    document.getElementById('serverIp').textContent = SERVER_IP;
    function copyIp(){ navigator.clipboard.writeText(SERVER_IP).then(()=> alert('IP скопирован: ' + SERVER_IP)); }
    document.getElementById('copyIp').addEventListener('click', copyIp);
    document.getElementById('copyIp2').addEventListener('click', copyIp);
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>

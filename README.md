<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SkinStrike — Магазин Скинов</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <!-- Навбар -->
  <header>
    <div class="logo">SkinStrike</div>
    <nav>
      <a href="#">Главная</a>
      <a href="#">Скины</a>
      <a href="https://t.me/sbyxha" target="_blank">Связаться: @sbyxha</a>
    </nav>
  </header>

  <!-- Хедер -->
  <section class="hero">
    <h1>Добро пожаловать в SkinStrike</h1>
    <p>Лучшие скины CS:GO по цене 100,000 сум</p>
    <a href="#skins" class="btn">Смотреть скины</a>
  </section>

  <!-- Каталог -->
  <section id="skins" class="skins">
    <h2>🔥 Наши Скины</h2>
    <div class="cards">
      <div class="card">
        <img src="https://cdn.cloudflare.steamstatic.com/apps/csgo/images/skillgroups/icon5.png" alt="AK-47">
        <h3>AK-47 | Redline</h3>
        <p class="price">100,000 сум</p>
        <button class="buy-btn">Купить</button>
      </div>
      <div class="card">
        <img src="https://cdn.cloudflare.steamstatic.com/apps/csgo/images/skillgroups/icon7.png" alt="AWP">
        <h3>AWP | Asiimov</h3>
        <p class="price">100,000 сум</p>
        <button class="buy-btn">Купить</button>
      </div>
      <div class="card">
        <img src="https://cdn.cloudflare.steamstatic.com/apps/csgo/images/skillgroups/icon8.png" alt="M4A4">
        <h3>M4A4 | Howl</h3>
        <p class="price">100,000 сум</p>
        <button class="buy-btn">Купить</button>
      </div>
    </div>
  </section>

  <!-- Футер -->
  <footer>
    <p>© 2025 SkinStrike | Контакт: <a href="https://t.me/sbyxha">@sbyxha</a></p>
  </footer>
</body>
</html>
/* Общий стиль */
body {
  margin: 0;
  font-family: 'Segoe UI', sans-serif;
  background: #0d0d0d;
  color: #fff;
}

/* Хедер */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 40px;
  background: #111;
  box-shadow: 0 0 15px #8a2be2;
  position: sticky;
  top: 0;
}

header .logo {
  font-size: 24px;
  font-weight: bold;
  color: #8a2be2;
}

header nav a {
  margin-left: 20px;
  text-decoration: none;
  color: #ccc;
  transition: 0.3s;
}

header nav a:hover {
  color: #8a2be2;
}

/* Hero */
.hero {
  text-align: center;
  padding: 100px 20px;
  background: linear-gradient(to bottom, #111, #0d0d0d);
}

.hero h1 {
  font-size: 48px;
  color: #fff;
  text-shadow: 0 0 15px #8a2be2;
}

.hero p {
  font-size: 18px;
  margin-top: 10px;
  color: #bbb;
}

.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 12px 25px;
  background: #8a2be2;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  transition: 0.3s;
}

.btn:hover {
  background: #a64dff;
  box-shadow: 0 0 15px #8a2be2;
}

/* Каталог */
.skins {
  padding: 60px 20px;
  text-align: center;
}

.skins h2 {
  font-size: 32px;
  margin-bottom: 40px;
  text-shadow: 0 0 10px #8a2be2;
}

.cards {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 25px;
}

.card {
  background: #1a1a1a;
  border-radius: 12px;
  padding: 20px;
  width: 260px;
  box-shadow: 0 0 15px rgba(138, 43, 226, 0.4);
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 0 25px rgba(138, 43, 226, 0.8);
}

.card img {
  width: 100%;
  border-radius: 8px;
}

.card h3 {
  margin: 15px 0 10px;
  font-size: 20px;
}

.price {
  font-size: 18px;
  color: #8a2be2;
  margin-bottom: 15px;
}

.buy-btn {
  padding: 10px 20px;
  background: #8a2be2;
  color: #fff;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
  transition: 0.3s;
}

.buy-btn:hover {
  background: #a64dff;
  box-shadow: 0 0 15px #8a2be2;
}

/* Футер */
footer {
  text-align: center;
  padding: 20px;
  background: #111;
  color: #888;
  margin-top: 50px;
}

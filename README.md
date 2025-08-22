<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SkinStrike - Магазин CS:GO скинов</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gradient-to-b from-gray-900 to-gray-800 text-white font-sans">

  <!-- Хедер -->
  <header class="bg-gray-900 shadow-lg sticky top-0 z-50">
    <div class="container mx-auto flex justify-between items-center p-4">
      <h1 class="text-3xl font-extrabold text-cyan-400">SkinStrike</h1>
      <nav class="space-x-6">
        <a href="#skins" class="hover:text-cyan-400 transition">Скины</a>
        <a href="#cart" class="hover:text-cyan-400 transition">Корзина (<span id="cart-count">0</span>)</a>
        <a href="#about" class="hover:text-cyan-400 transition">О нас</a>
        <a href="#contacts" class="hover:text-cyan-400 transition">Контакты</a>
      </nav>
    </div>
  </header>

  <!-- Главный баннер -->
  <section class="text-center py-20 bg-gradient-to-r from-cyan-500 via-blue-500 to-purple-600">
    <h2 class="text-5xl font-extrabold mb-4 text-white">Продажа лучших скинов CS:GO</h2>
    <p class="text-lg mb-6 text-gray-100">Купи дешёвые скины по выгодной цене прямо сейчас!</p>
    <a href="#skins" class="bg-cyan-500 hover:bg-cyan-600 text-black px-6 py-3 rounded-xl font-bold transition shadow-lg">Перейти в магазин</a>
  </section>

  <!-- Секция скинов -->
  <section id="skins" class="container mx-auto py-16 px-4">
    <h3 class="text-4xl font-bold text-center mb-12 text-cyan-400">Популярные скины</h3>
    <div class="grid md:grid-cols-3 gap-10">

      <!-- Карточка скина 1 -->
      <div class="bg-gray-800 rounded-3xl shadow-xl hover:shadow-cyan-500/50 transition overflow-hidden transform hover:scale-105">
        <img src="ТВОЕ_ИЗОБРАЖЕНИЕ_1" alt="Название скина 1" class="w-full h-52 object-contain bg-gray-900 p-2">
        <div class="p-5">
          <h4 class="text-xl font-bold text-cyan-400 mb-2">Название скина 1</h4>
          <p class="text-cyan-200 font-semibold mb-4">100.000 s'om</p>
          <button onclick="addToCart('Название скина 1', 100000)" class="w-full bg-cyan-500 hover:bg-cyan-600 text-black font-bold py-3 px-4 rounded-2xl transition shadow-md">В корзину</button>
        </div>
      </div>

      <!-- Карточка скина 2 -->
      <div class="bg-gray-800 rounded-3xl shadow-xl hover:shadow-cyan-500/50 transition overflow-hidden transform hover:scale-105">
        <img src="ТВОЕ_ИЗОБРАЖЕНИЕ_2" alt="Название скина 2" class="w-full h-52 object-contain bg-gray-900 p-2">
        <div class="p-5">
          <h4 class="text-xl font-bold text-cyan-400 mb-2">Название скина 2</h4>
          <p class="text-cyan-200 font-semibold mb-4">50.000 s'om</p>
          <button onclick="addToCart('Название скина 2', 50000)" class="w-full bg-cyan-500 hover:bg-cyan-600 text-black font-bold py-3 px-4 rounded-2xl transition shadow-md">В корзину</button>
        </div>
      </div>

      <!-- Карточка скина 3 -->
      <div class="bg-gray-800 rounded-3xl shadow-xl hover:shadow-cyan-500/50 transition overflow-hidden transform hover:scale-105">
        <img src="ТВОЕ_ИЗОБРАЖЕНИЕ_3" alt="Название скина 3" class="w-full h-52 object-contain bg-gray-900 p-2">
        <div class="p-5">
          <h4 class="text-xl font-bold text-cyan-400 mb-2">Название скина 3</h4>
          <p class="text-cyan-200 font-semibold mb-4">110.000 s'om</p>
          <button onclick="addToCart('Название скина 3', 110000)" class="w-full bg-cyan-500 hover:bg-cyan-600 text-black font-bold py-3 px-4 rounded-2xl transition shadow-md">В корзину</button>
        </div>
      </div>

    </div>
  </section>

  <!-- Корзина -->
  <section id="cart" class="bg-gray-800 py-16 px-4">
    <div class="container mx-auto">
      <h3 class="text-3xl font-bold text-center mb-6 text-cyan-400">Корзина</h3>
      <div id="cart-items" class="text-gray-300 text-lg text-center">Корзина пуста</div>
      <div id="cart-total" class="text-center mt-6 text-xl font-bold text-cyan-400"></div>
      <div class="text-center mt-6">
        <button onclick="checkout()" class="bg-cyan-500 hover:bg-cyan-600 text-black font-bold py-3 px-6 rounded-2xl transition shadow-md">Оплатить</button>
      </div>
    </div>
  </section>

  <!-- О нас -->
  <section id="about" class="bg-gray-900 py-16 px-4">
    <div class="container mx-auto text-center">
      <h3 class="text-3xl font-bold mb-6 text-cyan-400">О нас</h3>
      <p class="max-w-2xl mx-auto text-gray-300">SkinStrike – это платформа для покупки доступных скинов CS:GO. Мы предлагаем только проверенные и безопасные сделки, чтобы ты мог наслаждаться игрой с крутыми скинами.</p>
    </div>
  </section>

  <!-- Контакты -->
  <section id="contacts" class="bg-gray-900 text-white py-10">
    <div class="container mx-auto text-center">
      <h2 class="text-2xl font-bold mb-4 text-cyan-400">Связаться со мной по поводу сделок</h2>
      <p class="mb-2">Пиши в Telegram:</p>
      <a href="https://t.me/sbyxha" 
         class="bg-cyan-500 text-black px-6 py-2 rounded-lg hover:bg-cyan-600 transition shadow-md">
         📩 Мой Telegram (@sbyxha)
      </a>
    </div>
  </section>

  <!-- Футер -->
  <footer class="bg-gray-900 text-center p-6 text-gray-400">
    © 2025 SkinStrike. Все права защищены.
  </footer>

  <script>
    let cart = [];

    function addToCart(name, price) {
      cart.push({ name, price });
      updateCart();
    }

    function updateCart() {
      const cartItemsDiv = document.getElementById('cart-items');
      const cartCount = document.getElementById('cart-count');
      const cartTotal = document.getElementById('cart-total');

      if (cart.length === 0) {
        cartItemsDiv.innerHTML = "Корзина пуста";
        cartTotal.innerHTML = "";
        cartCount.innerText = 0;
        return;
      }

      cartItemsDiv.innerHTML = cart.map(item => `<p>${item.name} - $${item.price}</p>`).join("");
      const total = cart.reduce((sum, item) => sum + item.price, 0);
      cartTotal.innerHTML = `Итого: $${total}`;
      cartCount.innerText = cart.length;
    }

    function checkout() {
      if (cart.length === 0) {
        alert("Корзина пуста!");
        return;
      }
      alert("Спасибо за покупку! (Оплата в демо-режиме)");
      cart = [];
      updateCart();
    }
  </script>
</body>
</html>

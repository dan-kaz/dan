<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Интернет-магазин</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <h1>Мой Интернет-Магазин</h1>
    <div class="cart">
      🛒 Корзина: <span id="cart-count">0</span>
    </div>
  </header>

  <!-- Реклама сверху -->
  <div class="ad-block">
    <!-- Вставьте сюда рекламный код -->
  </div>

  <nav>
    <button onclick="filterItems('all')">Все</button>
    <button onclick="filterItems('electronics')">Электроника</button>
    <button onclick="filterItems('clothing')">Одежда</button>
  </nav>

  <main id="catalog">
    <div class="item electronics">
      <h2>Смартфон</h2>
      <p>Цена: 20 000 ₽</p>
      <button onclick="addToCart('Смартфон', 20000)">В корзину</button>
    </div>
    <div class="item clothing">
      <h2>Футболка</h2>
      <p>Цена: 1 000 ₽</p>
      <button onclick="addToCart('Футболка', 1000)">В корзину</button>
    </div>
    <div class="item electronics">
      <h2>Наушники</h2>
      <p>Цена: 3 000 ₽</p>
      <button onclick="addToCart('Наушники', 3000)">В корзину</button>
    </div>
  </main>

  <!-- Реклама снизу -->
  <div class="ad-block">
    <!-- Вставьте сюда рекламный код -->
  </div>

  <footer>
    <p>© 2025 Мой Магазин</p>
  </footer>

  <script>
    let cart = [];

    function filterItems(category) {
      const items = document.querySelectorAll('.item');
      items.forEach(item => {
        if (category === 'all' || item.classList.contains(category)) {
          item.style.display = 'block';
        } else {
          item.style.display = 'none';
        }
      });
    }

    function addToCart(name, price) {
      cart.push({ name, price });
      document.getElementById('cart-count').textContent = cart.length;
      alert(`${name} добавлен(а) в корзину!`);
    }
  </script>
</body>
</html>

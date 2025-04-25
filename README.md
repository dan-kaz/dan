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
    </div>
    <div class="item clothing">
      <h2>Футболка</h2>
      <p>Цена: 1 000 ₽</p>
    </div>
    <div class="item electronics">
      <h2>Наушники</h2>
      <p>Цена: 3 000 ₽</p>
    </div>
    <!-- Добавьте больше товаров -->
  </main>

  <!-- Реклама снизу -->
  <div class="ad-block">
    <!-- Вставьте сюда рекламный код -->
  </div>

  <footer>
    <p>© 2025 Мой Магазин</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>


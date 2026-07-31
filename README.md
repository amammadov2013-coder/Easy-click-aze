# Easy-click-aze
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trendyol Clone</title>
  <!-- Подключение Tailwind CSS через CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: '#f27a1a', // Фирменный оранжевый цвет Trendyol
          }
        }
      }
    }
  </script>
</head>
<body class="bg-gray-50 text-gray-800 font-sans">

  <!-- Верхняя шапка (Header) -->
  <header class="bg-white border-b sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 py-3 flex items-center justify-between gap-4">
      
      <!-- Логотип -->
      <a href="#" class="text-3xl font-extrabold text-brand tracking-tight">trendyol</a>

      <!-- Строка поиска -->
      <div class="flex-1 max-w-2xl relative">
        <input 
          type="text" 
          placeholder="Ищите бренд, категорию или товар..." 
          class="w-full bg-gray-100 border border-transparent focus:border-brand focus:bg-white rounded-md py-2.5 pl-4 pr-10 text-sm outline-none transition"
        >
        <button class="absolute right-3 top-2.5 text-brand font-bold">
          🔍
        </button>
      </div>

      <!-- Пользовательское меню -->
      <div class="flex items-center space-x-6 text-sm font-medium">
        <a href="#" class="hover:text-brand flex items-center gap-1">👤 Войти</a>
        <a href="#" class="hover:text-brand flex items-center gap-1">♡ Избранное</a>
        <a href="#" class="hover:text-brand flex items-center gap-1 bg-gray-100 px-3 py-2 rounded-md">🛒 Корзина</a>
      </div>
    </div>

    <!-- Категории -->
    <nav class="border-t">
      <div class="max-w-7xl mx-auto px-4 flex justify-between overflow-x-auto text-sm font-semibold py-2.5 space-x-6 whitespace-nowrap">
        <a href="#" class="text-brand border-b-2 border-brand pb-1">ЖЕНЩИНАМ</a>
        <a href="#" class="hover:text-brand pb-1">МУЖЧИНАМ</a>
        <a href="#" class="hover:text-brand pb-1">ОБУВЬ И СУМКИ</a>
        <a href="#" class="hover:text-brand pb-1">ДЕТЯМ</a>
        <a href="#" class="hover:text-brand pb-1">ДОМ И ЖИЗНЬ</a>
        <a href="#" class="hover:text-brand pb-1">КОСМЕТИКА</a>
        <a href="#" class="hover:text-brand pb-1">ЭЛЕКТРОНИКА</a>
        <a href="#" class="text-red-600 font-bold hover:opacity-80 pb-1">СКИДКИ %</a>
      </div>
    </nav>
  </header>

  <!-- Главный баннер -->
  <section class="max-w-7xl mx-auto px-4 my-6">
    <div class="bg-gradient-to-r from-orange-500 to-amber-500 rounded-xl p-8 text-white flex justify-between items-center shadow-lg">
      <div>
        <span class="bg-black text-white text-xs px-2 py-1 rounded font-bold uppercase tracking-wider">Суперцена</span>
        <h1 class="text-3xl font-black mt-2">Мегараспродажа сезона</h1>
        <p class="mt-1 opacity-90">Скидки до 70% на популярные бренды одежды и обуви</p>
      </div>
      <button class="bg-white text-brand font-bold px-6 py-3 rounded-lg hover:bg-gray-100 transition shadow">
        Смотреть товары
      </button>
    </div>
  </section>

  <!-- Каталог товаров -->
  <main class="max-w-7xl mx-auto px-4 mb-12">
    <h2 class="text-xl font-bold mb-4">Трендовые товары</h2>

    <!-- Сетка карточек -->
    <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-5 gap-4">

      <!-- Пример карточки товара 1 -->
      <div class="bg-white rounded-lg border hover:shadow-xl transition group overflow-hidden flex flex-col justify-between">
        <div>
          <div class="relative aspect-[3/4] bg-gray-200 overflow-hidden">
            <img src="https://via.placeholder.com/300x400" alt="Товар" class="w-full h-full object-cover group-hover:scale-105 transition duration-300">
            <span class="absolute top-2 left-2 bg-green-600 text-white text-[10px] font-bold px-1.5 py-0.5 rounded">Быстрая доставка</span>
          </div>
          <div class="p-3">
            <p class="text-xs font-bold text-gray-900">MANGO</p>
            <p class="text-xs text-gray-600 truncate mt-0.5">Оверсайз худи из хлопка</p>
            
            <div class="flex items-center gap-1 mt-2">
              <span class="text-yellow-400 text-xs">★</span>
              <span class="text-xs font-semibold">4.8</span>
              <span class="text-[10px] text-gray-400">(1,240)</span>
            </div>
          </div>
        </div>

        <div class="p-3 pt-0">
          <div class="mt-2">
            <span class="text-xs text-gray-400 line-through">2 990 ₽</span>
            <p class="text-base font-bold text-brand">1 890 ₽</p>
          </div>
        </div>
      </div>

      <!-- Повторите карточки при необходимости -->

    </div>
  </main>

</body>
</html>

<!DOCTYPE html>
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CK Shop - trust to ck company</title>
  <style>
    body {
      font-family: Tahoma;
      direction: rtl;
      margin: 0;
      padding: 0;
      background-color: #0e1013;
      color: #fff;
      transition: all 0.3s ease;
    }
    
    /* تم پیش‌فرض */
    :root {
      --primary-color: #3b82f6;
      --primary-dark: #1f2937;
      --primary-darker: #111827;
      --primary-light: #374151;
      --primary-lighter: #4b5563;
      --accent-color: #3b82f6;
      --text-color: #fff;
      --text-light: #d1d5db;
      --error-color: #ef4444;
      --success-color: #10b981;
    }
    
    /* تم سبز */
    .theme-green {
      --primary-color: #10b981;
      --primary-dark: #064e3b;
      --primary-darker: #022c22;
      --primary-light: #047857;
      --primary-lighter: #059669;
      --accent-color: #10b981;
    }
    
    /* تم آبی */
    .theme-blue {
      --primary-color: #3b82f6;
      --primary-dark: #1e40af;
      --primary-darker: #1e3a8a;
      --primary-light: #2563eb;
      --primary-lighter: #1d4ed8;
      --accent-color: #3b82f6;
    }
    
    /* تم قرمز */
    .theme-red {
      --primary-color: #ef4444;
      --primary-dark: #7f1d1d;
      --primary-darker: #450a0a;
      --primary-light: #dc2626;
      --primary-lighter: #b91c1c;
      --accent-color: #ef4444;
    }
    
    /* تم بنفش */
    .theme-purple {
      --primary-color: #8b5cf6;
      --primary-dark: #5b21b6;
      --primary-darker: #4c1d95;
      --primary-light: #7c3aed;
      --primary-lighter: #6d28d9;
      --accent-color: #8b5cf6;
    }
    
    /* تم مشکی */
    .theme-dark {
      --primary-color: #4b5563;
      --primary-dark: #111827;
      --primary-darker: #000000;
      --primary-light: #1f2937;
      --primary-lighter: #374151;
      --accent-color: #4b5563;
    }
    
    /* تم سورمه‌ای */
    .theme-indigo {
      --primary-color: #6366f1;
      --primary-dark: #3730a3;
      --primary-darker: #312e81;
      --primary-light: #4f46e5;
      --primary-lighter: #4338ca;
      --accent-color: #6366f1;
    }

    header {
      background-color: var(--primary-dark);
      padding: 20px;
      text-align: center;
      position: relative;
    }
    header input {
      width: 40%;
      padding: 10px;
      border: none;
      border-radius: 5px;
      margin-top: 10px;
      background-color: var(--primary-light);
      color: var(--text-color);
    }
    #cart {
      position: absolute;
      left: 20px;
      top: 20px;
      background: var(--primary-light);
      color: var(--text-color);
      padding: 10px;
      border-radius: 8px;
      font-size: 14px;
      box-shadow: 0 0 5px rgba(0,0,0,0.3);
    }
    #auth-btn {
      position: absolute;
      left: 150px;
      top: 20px;
      background: var(--primary-light);
      color: var(--text-color);
      padding: 10px;
      border-radius: 8px;
      font-size: 14px;
      box-shadow: 0 0 5px rgba(0,0,0,0.3);
      cursor: pointer;
    }
    #user-info {
      position: absolute;
      left: 150px;
      top: 20px;
      background: var(--primary-light);
      color: var(--text-color);
      padding: 10px;
      border-radius: 8px;
      font-size: 14px;
      box-shadow: 0 0 5px rgba(0,0,0,0.3);
      display: none;
    }
    nav {
  background-color: var(--primary-darker);
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
  padding: 15px;
  text-align: center;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 8px;
}

nav button {
  padding: 8px 14px 8px 14px;
  border: none;
  border-radius: 5px;
  background-color: var(--primary-light);
  color: var(--text-color);
  cursor: pointer;
  font-weight: bold;
  position: relative;
  padding-right: 40px;
  margin: 0;
  flex-shrink: 0;
}

nav button:hover {
  background-color: var(--primary-lighter);
}

nav button img {
  width: 24px;
  height: 24px;
  position: absolute;
  right: 10px;
  top: 50%;
  transform: translateY(-50%);
}

@media (max-width: 768px) {
  nav {
    padding: 10px;
    justify-content: flex-start;
    overflow-x: auto;
    white-space: nowrap;
    flex-wrap: nowrap;
  }
  
  nav button {
    padding: 6px 10px 6px 10px;
    padding-right: 30px;
    font-size: 12px;
    margin: 0;
  }
  
  nav button img {
    width: 18px;
    height: 18px;
    right: 5px;
  }
}

@media (max-width: 768px) {
  nav button {
    padding: 6px 10px 6px 10px;
    padding-right: 30px;
    font-size: 12px;
    margin: 4px;
  }
  nav button img {
    width: 18px;
    height: 18px;
    right: 5px;
  }
}
    section {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 30px;
    }
    .product {
      background-color: var(--primary-dark);
      border: 1px solid var(--primary-light);
      border-radius: 8px;
      width: 250px;
      margin: 15px;
      padding: 15px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
      position: relative;
    }
    .product img {
      width: 100%;
      height: 150px;
      object-fit: contain;
      margin-bottom: 10px;
    }
    .product h3 {
      font-size: 16px;
      margin: 10px 0;
    }
    .product p {
      color: var(--text-light);
      margin-bottom: 10px;
    }
    .product button {
      background-color: var(--accent-color);
      color: white;
      border: none;
      padding: 8px 12px;
      border-radius: 5px;
      cursor: pointer;
    }
    footer {
      background-color: var(--primary-darker);
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 30px;
    }
    .social-icons {
      margin-top: 15px;
    }
    .social-icons a {
      margin: 0 10px;
      display: inline-block;
    }
    .social-icons img {
      width: 24px;
      height: 24px;
      vertical-align: middle;
      transition: transform 0.3s;
    }
    .social-icons img:hover {
      transform: scale(1.2);
    }
    .modal {
      display: none;
      position: fixed;
      z-index: 100;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(0,0,0,0.7);
    }
    .modal-content {
      background-color: var(--primary-dark);
      margin: 5% auto;
      padding: 20px;
      border-radius: 8px;
      width: 50%;
      position: relative;
    }
    .close {
      position: absolute;
      left: 15px;
      top: 10px;
      color: #aaa;
      font-size: 28px;
      font-weight: bold;
      cursor: pointer;
    }
    .close:hover {
      color: white;
    }
    #auth-form input, #payment-form input, #payment-form select {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: none;
      border-radius: 5px;
      background-color: var(--primary-light);
      color: var(--text-color);
    }
    #auth-form button, #payment-form button {
      width: 100%;
      padding: 10px;
      background-color: var(--accent-color);
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .error-message {
      color: var(--error-color);
      font-size: 14px;
      margin-top: 5px;
    }
    .success-message {
      color: var(--success-color);
      font-size: 14px;
      margin-top: 5px;
    }
    
    /* استایل انتخابگر تم */
    #theme-selector {
      position: absolute;
      right: 20px;
      top: 20px;
      background: var(--primary-light);
      color: var(--text-color);
      padding: 8px 12px;
      border-radius: 8px;
      font-size: 14px;
      box-shadow: 0 0 5px rgba(0,0,0,0.3);
      cursor: pointer;
      border: none;
    }
    
    #theme-selector option {
      background: var(--primary-dark);
      color: var(--text-color);
    }
    
    /* استایل برچسب NEW */
    .new-badge {
      position: absolute;
      top: 10px;
      right: 10px;
      background-color: #ff0000;
      color: white;
      padding: 4px 10px;
      border-radius: 15px;
      font-size: 12px;
      font-weight: bold;
      box-shadow: 0 2px 5px rgba(0,0,0,0.3);
      animation: pulse 1.5s infinite;
      z-index: 10;
    }
    
    /* استایل انیمیشن بازی‌ها */
    .game-item {
      animation: shake 0.8s infinite alternate;
    }
    
    /* انیمیشن‌ها */
    @keyframes pulse {
      0% { transform: scale(1); opacity: 1; }
      50% { transform: scale(1.1); opacity: 0.9; }
      100% { transform: scale(1); opacity: 1; }
    }
    
    @keyframes shake {
      0% { transform: rotate(-2deg); }
      25% { transform: rotate(2deg); }
      50% { transform: rotate(-2deg); }
      75% { transform: rotate(2deg); }
      100% { transform: rotate(-2deg); }
    }
    
    @media (max-width: 768px) {
      header input {
        width: 70%;
      }
      #cart, #auth-btn, #user-info, #theme-selector {
        position: static;
        display: block;
        margin: 10px auto;
        width: 80%;
        text-align: center;
      }
      .modal-content {
        width: 90%;
      }
      .product {
        width: 100%;
        margin: 10px 0;
      }
      nav button {
        padding: 6px 10px 6px 30px;
        font-size: 12px;
        margin: 4px;
      }
      nav button img {
        width: 18px;
        height: 18px;
        right: 5px;
      }
    }
    @media (max-width: 480px) {
      header h1 {
        font-size: 20px;
      }
      header p {
        font-size: 14px;
      }
      nav {
        overflow-x: auto;
        white-space: nowrap;
        text-align: left;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>CK Shop - trust to ck company</h1>
    <p>فروش تخصصی اشتراک‌های دیجیتال و بازی‌ها</p>
    <input type="text" id="search" placeholder="جستجو در محصولات...">
    
    <select id="theme-selector" onchange="changeTheme(this.value)">
      <option value="default">تم پیش‌فرض</option>
      <option value="green">تم سبز</option>
      <option value="blue">تم آبی</option>
      <option value="red">تم قرمز</option>
      <option value="purple">تم بنفش</option>
      <option value="dark">تم مشکی</option>
      <option value="indigo">تم سورمه‌ای</option>
    </select>
    
    <div id="auth-btn" onclick="showAuthModal()">ورود / عضویت</div>
    <div id="user-info">
      <span id="username-display"></span>
      <button onclick="logout()" style="margin-right: 10px; background: var(--error-color); color: white; border: none; padding: 3px 8px; border-radius: 5px; cursor: pointer; font-size: 12px;">خروج</button>
    </div>
    <div id="cart">
      سبد خرید: <span id="cart-count">۰</span> مورد - مجموع: <span id="cart-total">۰</span> تومان
      <button onclick="checkout()" style="margin-right: 10px; background: var(--accent-color); color: white; border: none; padding: 5px 10px; border-radius: 5px; cursor: pointer;">پرداخت</button>
    </div>
  </header>

  <div id="auth-modal" class="modal">
    <div class="modal-content">
      <span class="close">&times;</span>
      <h2>ورود / عضویت</h2>
      <form id="auth-form">
        <div id="login-fields">
          <input type="text" id="login-username" placeholder="نام کاربری یا ایمیل" required>
          <input type="password" id="login-password" placeholder="رمز عبور" required>
          <div id="login-error" class="error-message"></div>
          <button type="button" onclick="login()">ورود</button>
          <p>کاربر جدید هستید؟ <a href="#" id="show-register">ثبت نام کنید</a></p>
        </div>
        <div id="register-fields" style="display:none">
          <input type="text" id="register-fullname" placeholder="نام کامل" required>
          <input type="email" id="register-email" placeholder="ایمیل" required>
          <input type="text" id="register-username" placeholder="نام کاربری" required>
          <input type="password" id="register-password" placeholder="رمز عبور" required>
          <input type="password" id="register-confirm" placeholder="تکرار رمز عبور" required>
          <div id="register-error" class="error-message"></div>
          <div id="register-success" class="success-message"></div>
          <button type="button" onclick="register()">ثبت نام</button>
          <p>قبلا ثبت نام کرده‌اید؟ <a href="#" id="show-login">ورود</a></p>
        </div>
      </form>
    </div>
  </div>
<nav>
  <button onclick="filterCategory('همه')"><img src="https://cdn-icons-png.flaticon.com/512/60/60992.png" alt="All">همه</button>
  <button onclick="filterCategory('Xbox')"><img src="https://upload.wikimedia.org/wikipedia/commons/f/f9/Xbox_one_logo.svg" alt="Xbox">Xbox</button>
  <button onclick="filterCategory('PlayStation')"><img src="https://upload.wikimedia.org/wikipedia/commons/0/00/PlayStation_logo.svg" alt="PlayStation">PS Plus</button>
  <button onclick="filterCategory('Netflix')"><img src="https://upload.wikimedia.org/wikipedia/commons/7/75/Netflix_icon.svg" alt="Netflix">Netflix</button>
  <button onclick="filterCategory('Spotify')"><img src="https://upload.wikimedia.org/wikipedia/commons/1/19/Spotify_logo_without_text.svg" alt="Spotify">Spotify</button>
  <button onclick="filterCategory('Apple')"><img src="https://upload.wikimedia.org/wikipedia/commons/f/fa/Apple_logo_black.svg" alt="Apple">Apple Music</button>
  <button onclick="filterCategory('EA')"><img src="https://upload.wikimedia.org/wikipedia/commons/6/6f/EA_Sports_monochrome_logo.svg" alt="EA">EA Play</button>
  <button onclick="filterCategory('Telegram')"><img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram">Telegram</button>
  <button onclick="filterCategory('بازی')"><img src="https://cdn-icons-png.flaticon.com/512/686/686589.png" alt="Games">بازی‌ها</button>
</nav>
  <section id="products"></section>

  <footer>
    <p>تمامی حقوق محفوظ است &copy; 2025 - CK Shop</p>
    <div class="social-icons">
      <a href="https://t.me/ckoori" target="_blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg" alt="Telegram">
      </a>
      <a href="https://www.instagram.com/ckooroshi?igsh=d3dmeTAybThiYnV3" target="_blank">
        <img src="https://upload.wikimedia.org/wikipedia/commons/e/e7/Instagram_logo_2016.svg" alt="Instagram">
      </a>
    </div>
  </footer>

  <script>
    // داده‌های محصولات
    const products = [
      // محصولات تلگرام
      { name: 'Telegram Premium - 1 ماهه', price: 120000, category: 'Telegram' },
      { name: 'Telegram Premium - 3 ماهه', price: 320000, category: 'Telegram' },
      { name: 'Telegram Premium - 6 ماهه', price: 600000, category: 'Telegram' },
      { name: 'Telegram Premium - 12 ماهه', price: 1100000, category: 'Telegram' },
      
      // بقیه محصولات
      { name: 'Game Pass Ultimate - 1 ماهه', price: 220000, category: 'Xbox' },
      { name: 'Game Pass Ultimate - 3 ماهه', price: 580000, category: 'Xbox' },
      { name: 'Game Pass Ultimate - 6 ماهه', price: 1100000, category: 'Xbox' },
      { name: 'Game Pass Ultimate - 12 ماهه', price: 2000000, category: 'Xbox' },
      { name: 'Game Pass Ultimate - 2 ساله', price: 3700000, category: 'Xbox' },
      { name: 'PS Plus Deluxe - 1 ماهه', price: 180000, category: 'PlayStation' },
      { name: 'PS Plus Deluxe - 3 ماهه', price: 450000, category: 'PlayStation' },
      { name: 'PS Plus Deluxe - 6 ماهه', price: 900000, category: 'PlayStation' },
      { name: 'PS Plus Deluxe - 12 ماهه', price: 1700000, category: 'PlayStation' },
      { name: 'نتفلیکس پرمیوم - 1 ماهه', price: 215000, category: 'Netflix' },
      { name: 'Apple Music - 1 ماهه', price: 289000, category: 'Apple' },
      { name: 'Spotify Premium - 1 ماهه', price: 143000, category: 'Spotify' },
      { name: 'EA Play - 1 ماهه', price: 180000, category: 'EA' },
      { name: 'EA Play - 12 ماهه', price: 1100000, category: 'EA' },
      { name: 'FC 25', price: 2350000, category: 'بازی' },
      { name: 'Call of Duty: Modern Warfare III', price: 3200000, category: 'بازی' },
      { name: 'GTA V (نسخه کامل)', price: 2700000, category: 'بازی' },
      { name: 'Red Dead Redemption 2', price: 2500000, category: 'بازی' },
      { name: 'Fortnite V-Bucks Pack', price: 980000, category: 'بازی' },
      { name: 'Elden Ring', price: 2950000, category: 'بازی' },
      { name: 'Cyberpunk 2077', price: 2300000, category: 'بازی' },
      { name: 'God of War: Ragnarok', price: 3300000, category: 'بازی' },
      { name: 'Spider-Man 2 (PS5)', price: 3500000, category: 'بازی' },
      { name: 'Assassin\'s Creed Shadows', price: 3100000, category: 'بازی' },
      { name: 'The Crew Motorfest', price: 2800000, category: 'بازی' },
      { name: 'Need for Speed Heat', price: 1900000, category: 'بازی' },
      { name: 'Gotham Knights', price: 2400000, category: 'بازی' }
    ];

    const productImages = {
      "Telegram": "https://upload.wikimedia.org/wikipedia/commons/8/82/Telegram_logo.svg",
      "Xbox": "https://assets.xboxservices.com/assets/dd/a1/dda1aa1d-99f2-470b-9773-710eabf849e0.jpg",
      "PlayStation": "https://image.api.playstation.com/vulcan/ap/rnd/202204/0810/803Pm8uJoZ2Cl9fJPvTaXHqG.png",
      "Netflix": "https://upload.wikimedia.org/wikipedia/commons/7/75/Netflix_icon.svg",
      "Apple": "https://upload.wikimedia.org/wikipedia/commons/f/fa/Apple_logo_black.svg",
      "Spotify": "https://upload.wikimedia.org/wikipedia/commons/1/19/Spotify_logo_without_text.svg",
      "EA": "https://media.contentapi.ea.com/content/dam/eacom/images/2020/06/ea-featured-image-ea-play.jpg.adapt.crop191x100.1200w.jpg",
      "FC 25": "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQPMi1lcaxCdbtCyZAyxqYr9DTwRVYJTkhAag&s",
      "Call of Duty: Modern Warfare III": "https://store-images.s-microsoft.com/image/apps.55183.14623575291286193.52ecceb7-ac9f-47e8-a29f-30ab63f33131.048bddb8-7ab3-4ba2-85b8-6acb95ee03b5",
      "GTA V (نسخه کامل)": "https://upload.wikimedia.org/wikipedia/en/a/a5/Grand_Theft_Auto_V.png",
      "Red Dead Redemption 2": "https://upload.wikimedia.org/wikipedia/en/4/44/Red_Dead_Redemption_II.jpg",
      "Fortnite V-Bucks Pack": "https://m.media-amazon.com/images/M/MV5BMTZlMmIxM2EtN2Y4Zi00M2ZhLTk3NzgtNjJmZTU0MTQ3YjcwXkEyXkFqcGc@._V1_FMjpg_UX1000_.jpg",
      "Elden Ring": "https://upload.wikimedia.org/wikipedia/en/b/b9/Elden_Ring_Box_art.jpg",
      "Cyberpunk 2077": "https://upload.wikimedia.org/wikipedia/en/9/9f/Cyberpunk_2077_box_art.jpg",
      "God of War: Ragnarok": "https://upload.wikimedia.org/wikipedia/en/e/ee/God_of_War_Ragnar%C3%B6k_cover.jpg",
      "Spider-Man 2 (PS5)": "https://i.etsystatic.com/35198957/r/il/39a9a9/5388247403/il_570xN.5388247403_lkuv.jpg",
      "Assassin's Creed Shadows": "https://assets-prd.ignimgs.com/2024/05/15/acshadows-1715789601294.jpg",
      "The Crew Motorfest":"https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcSvy4zKFk4fH7HL2B4Z0wlhT4OpOw6mbHjNfRbxco-Nzk3R1BIsAh9WoUDhxjcwihhrCRN3",
      "Need for Speed Heat": "https://store-images.s-microsoft.com/image/apps.26776.69435230515002378.477c7a96-5d17-45ec-95c2-a2739146b68d.b0d37a76-e4fa-495e-abac-6697ee4b5887",
      "Gotham Knights": "https://cdn.myportfolio.com/104baae407c3bf6924ab16701d4f9991/f076f5f4-0a36-407d-ac41-80d92936564a_rw_1920.jpg?h=e3d15d0c00c0a209fda76177efafa55f",
    };

    // متغیرهای عمومی
    let cartCount = 0;
    let cartTotal = 0;
    let currentUser = null;

    // المنت‌های DOM
    const container = document.getElementById("products");
    const searchInput = document.getElementById("search");
    const authBtn = document.getElementById("auth-btn");
    const userInfo = document.getElementById("user-info");
    const usernameDisplay = document.getElementById("username-display");
    const themeSelector = document.getElementById("theme-selector");

    // تغییر تم
    function changeTheme(theme) {
      // حذف تمام کلاس‌های تم از body
      document.body.classList.remove(
        'theme-green', 'theme-blue', 'theme-red', 
        'theme-purple', 'theme-dark', 'theme-indigo'
      );
      
      // اضافه کردن تم انتخاب شده
      if (theme !== 'default') {
        document.body.classList.add(`theme-${theme}`);
      }
      
      // ذخیره تم انتخاب شده
      localStorage.setItem('ckShopTheme', theme);
    }

    // بارگذاری تم ذخیره شده
    function loadTheme() {
      const savedTheme = localStorage.getItem('ckShopTheme') || 'default';
      themeSelector.value = savedTheme;
      changeTheme(savedTheme);
    }

    // سیستم کاربران
    function getUsers() {
      return JSON.parse(localStorage.getItem('ckShopUsers')) || [];
    }

    function saveUsers(users) {
      localStorage.setItem('ckShopUsers', JSON.stringify(users));
    }

    function getCurrentUser() {
      return JSON.parse(localStorage.getItem('ckShopCurrentUser'));
    }

    function setCurrentUser(user) {
      localStorage.setItem('ckShopCurrentUser', JSON.stringify(user));
    }

    function clearCurrentUser() {
      localStorage.removeItem('ckShopCurrentUser');
    }

    // ثبت نام کاربر جدید
    function register() {
      const fullname = document.getElementById("register-fullname").value.trim();
      const email = document.getElementById("register-email").value.trim();
      const username = document.getElementById("register-username").value.trim();
      const password = document.getElementById("register-password").value;
      const confirm = document.getElementById("register-confirm").value;
      
      const errorElement = document.getElementById("register-error");
      const successElement = document.getElementById("register-success");
      
      errorElement.textContent = "";
      successElement.textContent = "";
      
      // اعتبارسنجی
      if (!fullname || !email || !username || !password || !confirm) {
        errorElement.textContent = "لطفا تمام فیلدها را پر کنید";
        return;
      }
      
      if (password !== confirm) {
        errorElement.textcontent = "رمز عبور و تکرار آن مطابقت ندارند";
        return;
      }
      
      if (password.length < 6) {
        errorElement.textContent = "رمز عبور باید حداقل ۶ کاراکتر باشد";
        return;
      }
      
      const users = getUsers();
      
      // بررسی تکراری نبودن نام کاربری و ایمیل
      if (users.some(u => u.username === username)) {
        errorElement.textContent = "این نام کاربری قبلا ثبت شده است";
        return;
      }
      
      if (users.some(u => u.email === email)) {
        errorElement.textContent = "این ایمیل قبلا ثبت شده است";
        return;
      }
      
      // ثبت کاربر جدید
      const newUser = {
        id: Date.now(),
        fullname,
        email,
        username,
        password,
        joinDate: new Date().toISOString()
      };
      
      users.push(newUser);
      saveUsers(users);
      
      successElement.textContent = "ثبت نام با موفقیت انجام شد! اکنون می‌توانید وارد شوید";
      
      // نمایش فرم ورود
      document.getElementById('register-fields').style.display = 'none';
      document.getElementById('login-fields').style.display = 'block';
    }

    // ورود کاربر
    function login() {
      const username = document.getElementById("login-username").value.trim();
      const password = document.getElementById("login-password").value;
      
      const errorElement = document.getElementById("login-error");
      errorElement.textContent = "";
      
      if (!username || !password) {
        errorElement.textContent = "لطفا نام کاربری و رمز عبور را وارد کنید";
        return;
      }
      
      const users = getUsers();
      const user = users.find(u => (u.username === username || u.email === username) && u.password === password);
      
      if (!user) {
        errorElement.textContent = "نام کاربری یا رمز عبور اشتباه است";
        return;
      }
      
      // ذخیره کاربر فعلی
      setCurrentUser(user);
      currentUser = user;
      
      // به‌روزرسانی UI
      updateUserUI();
      closeAuthModal();
    }

    // خروج کاربر
    function logout() {
      clearCurrentUser();
      currentUser = null;
      updateUserUI();
    }

    // به‌روزرسانی نمایش وضعیت کاربر
    function updateUserUI() {
      const user = getCurrentUser();
      
      if (user) {
        authBtn.style.display = 'none';
        userInfo.style.display = 'block';
        usernameDisplay.textContent = `خوش آمدید ${user.fullname}`;
      } else {
        authBtn.style.display = 'block';
        userInfo.style.display = 'none';
      }
    }

    // مدیریت محصولات و سبد خرید
    function renderProducts(list) {
      container.innerHTML = '';
      list.forEach(p => {
        const card = document.createElement("div");
        card.className = "product";
        
        // اضافه کردن انیمیشن برای بازی‌ها
        if (p.category === 'بازی') {
          card.classList.add('game-item');
        }
        
        const img = productImages[p.name] || productImages[p.category] || '';
        
        card.innerHTML = `
          <img src="${img}" alt="logo">
          <span class="new-badge">NEW</span>
          <h3>${p.name}</h3>
          <p>قیمت: ${p.price.toLocaleString()} تومان</p>
          <button onclick="addToCart(${p.price})">افزودن به سبد</button>
        `;
        container.appendChild(card);
      });
    }

    function addToCart(price) {
      if (!currentUser) {
        alert('لطفا ابتدا وارد حساب کاربری خود شوید');
        showAuthModal();
        return;
      }
      
      cartCount++;
      cartTotal += price;
      document.getElementById("cart-count").textContent = cartCount;
      document.getElementById("cart-total").textContent = cartTotal.toLocaleString();
    }

    function filterCategory(category) {
      if (category === 'همه') {
        renderProducts(products);
      } else {
        const filtered = products.filter(p => p.category === category);
        renderProducts(filtered);
      }
    }

    function checkout() {
      if (!currentUser) {
        alert('لطفا ابتدا وارد حساب کاربری خود شوید');
        showAuthModal();
        return;
      }
      
      if (cartCount === 0) {
        alert('سبد خرید شما خالی است!');
        return;
      }
      
      const modal = document.createElement('div');
      modal.className = 'modal';
      modal.innerHTML = `
        <div class="modal-content" style="max-width: 500px;">
          <span class="close" onclick="document.body.removeChild(this.parentElement.parentElement)">&times;</span>
          <h2>تکمیل خرید</h2>
          <p>مجموع خرید: ${cartTotal.toLocaleString()} تومان</p>
          <form id="payment-form">
            <input type="text" placeholder="نام کامل" value="${currentUser.fullname}" required>
            <input type="tel" placeholder="شماره همراه" required>
            <select required>
              <option value="">روش پرداخت را انتخاب کنید</option>
              <option value="zarinpal">زرین پال</option>
              <option value="idpay">آیدی پی</option>
              <option value="card">کارت به کارت</option>
            </select>
            <button type="submit">پرداخت</button>
          </form>
        </div>
      `;
      
      document.body.appendChild(modal);
      document.getElementById('payment-form').addEventListener('submit', function(e) {
        e.preventDefault();
        alert('پرداخت با موفقیت انجام شد! سفارش شما ثبت گردید.');
        cartCount = 0;
        cartTotal = 0;
        document.getElementById("cart-count").textContent = '۰';
        document.getElementById("cart-total").textContent = '۰';
        document.body.removeChild(modal);
      });
    }

    // مدیریت مودال عضویت/ورود
    function showAuthModal() {
      document.getElementById('auth-modal').style.display = 'block';
    }

    function closeAuthModal() {
      document.getElementById('auth-modal').style.display = 'none';
    }

    // رویدادهای صفحه
    document.addEventListener('DOMContentLoaded', function() {
      // بارگذاری تم ذخیره شده
      loadTheme();
      
      // بررسی کاربر لاگین کرده
      currentUser = getCurrentUser();
      updateUserUI();
      
      // رویدادهای مودال عضویت/ورود
      document.querySelector('.close').onclick = closeAuthModal;
      document.getElementById('show-register').onclick = function(e) {
        e.preventDefault();
        document.getElementById('login-fields').style.display = 'none';
        document.getElementById('register-fields').style.display = 'block';
      };
      document.getElementById('show-login').onclick = function(e) {
        e.preventDefault();
        document.getElementById('register-fields').style.display = 'none';
        document.getElementById('login-fields').style.display = 'block';
      };
      
      // بستن مودال با کلیک خارج از آن
      window.onclick = function(event) {
        const modal = document.getElementById('auth-modal');
        if (event.target == modal) {
          modal.style.display = 'none';
        }
      };
    });

    // جستجوی محصولات
    searchInput.addEventListener("input", () => {
      const value = searchInput.value.trim();
      const filtered = products.filter(p => p.name.includes(value));
      renderProducts(filtered);
    });

    // نمایش اولیه محصولات
    renderProducts(products);
  </script>
</body>
</html>

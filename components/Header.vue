<template>
    <div class="container">
      <header class="navbar">
        <!-- Logo -->
        <div class="logo">
          <img src="https://static.ticimax.cloud/39045/uploads/editoruploads/bivagon.jpg" alt="Bivagon Logo" />
        </div>
   
        <!-- Menü -->
        <nav class="menu">
          <ul>
            <li><a href="#">Endüstriyel Mutfak Ekipmanları</a></li>
            <li><a href="#">Bıçaklar</a></li>
            <li><a href="#">Termoslar</a></li>
            <li><a href="#">Diğer Ürünler</a></li>
          </ul>
        </nav>
   
        <!-- İkonlar -->
        <div class="icons">
          <i class="fa fa-user"></i>
          <i class="fa fa-user-plus"></i>
          <i class="fa fa-search"></i>
          <i class="fa fa-shopping-cart"></i>
        </div>
      </header>
    </div>
  </template>
   
  <script setup>
  // Script kısmı boş bırakılabilir.
  </script>
   
  <style scoped>
  /* Genel Container */
  .container {
    max-width: 1200px;
    margin: 0 auto; /* Ortalamak için */
    padding: 0 400px; /* Kenarlardan içeri boşluk */
  }
   
  /* Navbar */
  .navbar {
    display: flex;
    flex-direction: column; /* Üst üste dizilim */
    align-items: center; /* Ortalamak için */
    padding: 20px 0;
    border-bottom: 1px solid #ddd;
    background-color: white;
    font-family: Arial, sans-serif;
  }
   
  /* Logo */
  .logo img {
    max-height: 120px; /* Logoyu görsele uygun boyutta ayarladık */
    margin-bottom: 60px; /* Menüyle aradaki boşluk */
  }
   
  /* Menü */
  .menu ul {
    list-style: none;
    display: flex;
    gap: 80px; /* Menü elemanları arasındaki boşluk */
    padding: 0;
    margin: 0;
  }
   
  .menu ul li {
    max-width: 200px; /* Uzun yazıların genişliğini sınırlar */
    text-align: center; /* Yazıları ortalar */
  }
   
  .menu ul li a {
    text-decoration: none;
    color: #333;
    font-size: 16px;
    font-weight: bold;
    white-space: nowrap; /* Yazıların alt alta gelmesini engeller */
    overflow: hidden; /* Taşma durumunda yazıyı gizler */
    text-overflow: ellipsis; /* Uzun yazılarda "..." ekler */
    transition: color 0.3s;
  }
   
  .menu ul li a:hover {
    color: #007bff;
  }
   
  /* İkonlar */
  .icons {
    display: flex;
    justify-content: center; /* İkonları ortalar */
    gap: 25px; /* İkonlar arasındaki boşluk */
    margin-top: 20px; /* Menü ile ikonlar arasındaki boşluk */
  }
   
  .icons i {
    font-size: 24px;
    color: #007bff;
    cursor: pointer;
  }
   
  /* Responsive Tasarım */
  @media screen and (max-width: 768px) {
    .menu ul {
      gap: 20px; /* Küçük ekranlarda daha dar boşluk */
    }
    .icons {
      gap: 15px;
    }
  }
  </style>

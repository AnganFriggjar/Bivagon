<template>
  <nav class="navbar">
  <!-- 1. buton için özel metin Header olarak belirleniyor -->
  <button v-for="n in 10" :key="n" @click="emitChange(n)">
   {{ 
        n === 1 
          ? 'Header' 
          : (n === 2 
              ? 'Footer' 
              : (n === 3 
                  ? 'Giriş Yap / Kayıt Ol' 
                  : n)) 
      }} <!-- 1. buton Header, 2. Footer, 3. Giriş Yap / Kayıt Ol olacak -->
  </button>
  </nav>
  </template>
   
  <script>
  export default {
    methods: {
      emitChange(n) {
        this.$emit("changeComponent", n); // Parent'a event gönder
      },
    },
  };
  </script>
   
  <style>
  .navbar {
    width: 200px;
    background-color: #f4f4f4;
    display: flex;
    flex-direction: column;
    padding: 10px;
  }
  button {
    margin-bottom: 10px;
    padding: 10px;
    background-color: #007bff;
    color: #fff;
    border: none;
    cursor: pointer;
  }
  button:hover {
    background-color: #0056b3;
  }
  </style>
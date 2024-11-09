<template>
    <div class="card">
      <img :src="icon_url" class="card-img-top" alt="Chuck Norris">
      <div class="card-body">
        <p class="card-text">{{ value }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChuckCard',
    props: {
      icon_url: String,
      value: String
    }
  };
  </script>
  
  <style scoped>
  .card {
    width: 100%;
    max-width: 18rem;
    margin: auto;
  }
  </style>
  
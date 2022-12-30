<template>
    <img class="profile" :src="image" alt="profile">
  </template>
  
  <script>
  export default {
    name: "ProfileImage",
    props:{
      image: String
    }
  }
  </script>
  
  <style>
  </style>
<script setup>
import { ref } from 'vue';

const user = ref({
  id: 1,
  avatar: 'https://www.w3schools.com/w3images/team2.jpg',
  name: 'Mai Cong Thanh',
  jobTitle: 'Software Engineer',
  university: 'Industrial University'
})


// const click = () => {
//   user.value.push({
//     id: user.value.length + 1,
//     name: 'new-item',
//     location: 'new-location'
//   })
// }
</script>

<template>
  <div>
    <h2 style="text-align:center">User Profile Card</h2>

    <div class="card">
      <img :src="user.avatar" alt="avatar" style="width:100%">
      <h1>{{ user.name }}</h1>
      <p>{{ user.jobTitle }}</p>
      <p>{{ user.university }}</p>
      <div style="margin: 24px 0;">
        <a href="#"><i class="fa fa-dribbble"></i></a>
        <a href="#"><i class="fa fa-twitter"></i></a>
        <a href="#"><i class="fa fa-linkedin"></i></a>
        <a href="#"><i class="fa fa-facebook"></i></a>
      </div>
      <p><button>Contact</button></p>
    </div>
  </div>
</template>

<style scoped></style>
<script setup>
import { ref } from 'vue'

</script>

<template>
  <div class="first-slide" id="first-slide">
      <span class="text-logo">Quizizy</span>
      <h2 class="welcome-text">Welcome to <span class="aws">AWS Cloud</span> Practitioner Knowledge Quiz</h2>
      <div class="input-btn">
          <form>
            <input type="text" placeholder="Please Enter Your Name" id="username-input" class="username-input" name="username" />
            <p id="empty-input"></p>
          </form>
          <button class="btn" id="start">Start</button>
      </div>
  </div>
</template>

<style scoped>
</style>

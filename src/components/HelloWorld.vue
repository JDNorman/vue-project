<script setup>
defineProps({
  welcomemsg: {
    type: String,
    required: true
  },
  submsg: {
    type: String,
    required: true
  },
})
</script>

<template>
  <div class="greetings">
    <h3>{{ welcomemsg }}</h3>
    <h1 class="yellow">
      CHOAM
    </h1>
    <h3 class="submsg text-purple disabled relative">{{ submsg }}</h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 5rem;
  position: relative;
  top: -10px;
  font-family: 'Made Tommy', serif;
}

.submsg {
  font-family: 'Playwrite CA';
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>

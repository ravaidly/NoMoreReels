<script lang="ts">
export default {
  data() {
    return {
      name: 'Vue.js'
    }
  },
  methods: {
    greet() {
      window.location.href = "https://www.youtube.com/watch?v=v7ScGV5128A";
    }
  }
};
</script>

<template>
  <div class="greetings">
    <h3>
      Type in a Public Account and click Submit to check their feed.
    </h3>
    <v-text-field label="Username"></v-text-field>
    <v-btn variant="flat" color="secondary" @click="greet">
      Submit
    </v-btn>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
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

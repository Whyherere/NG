<template>
  <div class="new-year">
    <h1>{{ GRU }}</h1>
    <input v-model="name" numb="Введите ваше имя" />
    <button @click="NG">Поздравление</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      GRU: 'С новым годом!',
      name: ''
    }
  },
  methods: {
    NG() {
      this.GRU = `С новым годом, ${this.name}!`
    }
  }
}
</script>

<style scoped>
.new-year {
  text-align: center;
}
h1 {
  font-size: 50px;
}
input {
  padding: 10px;
}
button {
  padding: 10px 20px;
  margin-top: 10px;
}
</style>
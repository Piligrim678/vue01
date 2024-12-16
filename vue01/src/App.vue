<script>
export default {
  data() {
    return {
      info: "Title!!!",
      anotherInfo: "Very good text",
    }
  },
  methods: {
    dataHandler(par = "AAAAAAA") {
      this.info = par
      this.anotherInfo = "Something new too"
    }
  }
}
</script>

<template>
  <h3>{{info}}</h3>
  <p>{{anotherInfo}}</p>

  <button type="button" @click="dataHandler()">Отправить</button>
</template>

<style scoped>
h3 {
  font-weight: lighter;
}
p {
  color: navy;
}
</style>

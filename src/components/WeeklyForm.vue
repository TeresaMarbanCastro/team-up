<template>
    <main class="main-container">
      <form>
        <ul class="checkbox-container">
          <li class="checkbox" v-for="(item, i) in items" :key="i">
            <label :for="item">{{item}}</label>
            <input type="checkbox" :id="item">
            <input type="text" placeholder="nota">
          </li>
        </ul>
      </form>

      <section>
      </section>
    </main>
</template>

<script>
export default {
  name: 'WeeklyForm',
  data() {
    return {
      items: ['Lunes', 'Martes', 'Miércoles', 'Jueves', 'Viernes', 'Sábado', 'Domingo']
    }
  },
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">

ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: flex;
  align-items: center;
  margin: 20px;
}
.checkbox input{
  height: 20px;
  width: 20px;
  margin: 0 5px 0 50;
  color:#42b983;
}
a {
  color: #42b983;
}
</style>

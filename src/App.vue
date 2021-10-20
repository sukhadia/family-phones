<template>
  <div id="app">
    <div class="container">
      <div class="item" v-for="(person, index) of people" :key="index">
        <p>
          <span>{{ person.name }}</span>
          <span>{{ person.phone }}</span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      people: [
        {
          name: "John",
          phone: "888-111-2222",
        },
        {
          name: "Michael",
          phone: "888-222-3333",
        },
        {
          name: "Ed",
          phone: "888-333-4444",
        },
        {
          name: "Ralph",
          phone: "888-444-5555",
        },
      ],
    };
  },
};
</script>

<style>
body,
html {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0;
  padding: 0;
}
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background: #2c3e50;
  width: 100%;
  height: 100%;
}
.container {
  list-style: none;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.item {
  width: 100%;
  border: 3px solid white;
  border-radius: 10px;
  /* padding: 0.75rem; */
  margin: 1rem 0;
  background: orangered;
  text-align: left;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-weight: 700;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  line-height: 1rem;
  box-sizing: border-box;
  max-width: 60%;
  padding: 0;
  max-height: 3rem;
}
.item p {
  /* border-radius: 3px; */
  width: 100%;
  min-height: 100%;
  display: flex;
  justify-content: space-between;
  background: orangered;
  color: white;
  padding: 0.75rem;
}
</style>

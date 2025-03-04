<template>
  <div>
    <header class="header">
      <h1 class="title">Dad Jokes</h1>
      <ul>
        <li>
          <nuxt-link to="/">Home</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/jokes">Jokes</nuxt-link>
        </li>
        <li>
          <nuxt-link to="/about">About</nuxt-link>
        </li>
      </ul>
    </header>
  </div>
</template>

<script>
  export default {
    name: 'AppHeader',
  }
</script>

<style >
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  border-bottom: 1px dotted #ccc;
  padding-bottom: 1rem;
}

.header .title {
  font-size: 3rem;
  color: #526488
}

.header ul {
display: flex;
list-style-type: none;
}

.header a {
  display: inline-block;
  background-color: #333;
  color: #fff;
  padding: 0.3rem;
  margin-right: 0.5rem;
}


</style>
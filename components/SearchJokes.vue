<template>
  <form @submit.prevent="onSubmit">
    <input type="text" v-model="text" placeholder="Search Jokes..." >
    <input type="submit" value="Search Jokes">
  </form>
</template>

<script>
  export default {
    name: "SearchJokes",
    data() {
      return {
        test: ""
      };
    },

    methods: {
      onSubmit() {
        this.$emit("search-text", this.text);
        this.text = "";
      }
    }
  };
</script>

<style scoped>
form{
  padding-left: 20px;
}

</style>

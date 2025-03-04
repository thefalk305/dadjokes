<template>
  <form @submit.prevent="onSubmit">
    <input type="text" v-model="text" placeholder="Search Jokes..." >
    <input type="submit" value="Search Jokes">
    <div>Page: </div>
  </form>
</template>

<script>
// const props = ([page]);
// console.log(props.page);
// const page = 0;

export default {

  name: "SearchJokes",
  data() {
    return {
      text: ""
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

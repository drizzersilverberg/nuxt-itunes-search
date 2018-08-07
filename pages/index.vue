<template lang="html">
  <div>
    <h1>Search iTunes</h1>
    <br/>
    <form @submit.prevent="submit">
      <input v-model="search" placeholder="Enter Artist Name" type="text" autofocus />
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      search: ''
    }
  },
  methods: {
    submit(event) {
      this.$router.push('/results/' + this.search)
    }
  }
}
</script>

<style lang="css" scoped>
* {
  text-align: center;
}
h1 {
  padding: 20px;
}
</style>

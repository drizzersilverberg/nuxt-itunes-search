<template>
  <section class="container">
    <div>
      <ToolBar/>
      <nuxt/>
    </div>
  </section>
</template>

<script>
import ToolBar from '~/components/ToolBar'
export default {
  components: {
    ToolBar
  }
}
</script>

<style>
</style>

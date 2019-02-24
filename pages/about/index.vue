<template>
  <section class="container">
    <div>
      <h1 class="my-title">This is about page!</h1>
      str1({{"<"+"br"+">"}}):
      <div v-html="str1"></div>
      <div>{{str1}}</div>
      <textarea v-model="str1"></textarea>
      <br>
      -------------------------------------------------
      <br>
      str2(\n):
      <div v-html="str2"></div>
      <div>{{str2}}</div>
      <textarea v-model="str2"></textarea>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      str1: "Hello <br> world",
      str2: "Hello \n world"
    }
  }
}
</script>

<style lang="stylus" scoped>
  h1
    color mainFontColor
  
</style>

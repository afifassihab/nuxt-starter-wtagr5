<template>
<h1 @click="toggleText"> {{ displayText }} </h1>
</template>

<script>
export default {
  data () {
    return {
      title: "Welcome to my blog",
      title2: "This is just a stackblitz test",
      displayText: "Welcome to my blog"
    }
  },
  methods: {
    toggleText() {
      if (this.displayText == this.title) {
        this.displayText = this.title2
      } else {
        this.displayText = this.title
      }
    }
  },
}
</script>

<style scoped>
h1 {
  cursor: pointer;
}
</style>
<template>
  <div>
    <sample-component :title="indexTitle">
      slot example
    </sample-component>
    <nuxt-link to="/about">About</nuxt-link>
  </div>
</template>
    

<script>
import Logo from '~/components/Logo.vue'
import SampleComponent from '~/components/Sample.vue'

export default {
  components: {
    Logo,
    SampleComponent
  },
  data() {
    return {
      indexTitle: 'Nuxt.js YEYYEY'
    }
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>

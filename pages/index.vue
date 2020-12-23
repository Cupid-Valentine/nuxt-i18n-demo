<template>
  <div class="container">
    <h1>{{ $t('home.title') }}</h1>
    <p>{{ $t('home.introduction') }}</p>
  </div>
</template>

<script>
export default {
  head() {
    return {
      title: 'home page',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'this is home page'
        },
        {
          hid: 'viewport',
          name: 'viewport',
          content: 'width=device-width, initial-scale=1.0'
        }
      ]
    }
  }
}
</script>

<style>
</style>

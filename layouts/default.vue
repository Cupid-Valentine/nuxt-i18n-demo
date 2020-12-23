<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="info">
      <b-navbar-brand href="#">NavBar</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse" />

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="/">Home</b-nav-item>
          <b-nav-item href="/about">about</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown text="Lang" right>
            <b-dropdown-item href="#">
              <nuxt-link :to="switchLocalePath('en')">English</nuxt-link>
            </b-dropdown-item>
            <b-dropdown-item href="#">
              <nuxt-link :to="switchLocalePath('zh')">中文</nuxt-link>
            </b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <Nuxt />
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  mounted() {
    // eslint-disable-next-line no-console
    console.log(this.$route)
  },
  methods: {},
}
</script>
<style>
.dropdown-item a {
  display: inline-block;
  width: 100%;
}
</style>

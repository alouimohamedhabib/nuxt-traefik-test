<template>
  <ul>
      <li><nuxt-link to="/"> Home page </nuxt-link></li>
      <li>
        <nuxt-link to="/contact"> Contact page </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/user/1345"> User page </nuxt-link>
      </li>
      <li>
        <nuxt-link to="/person">Person </nuxt-link>
      </li>
    </ul>
</template>

<script>
export default {
  ssr: true,
  async asyncData() {
    await console.log('Alert people Header component')
  },
}
</script>

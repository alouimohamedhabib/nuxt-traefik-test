<template>
  <div>
    <div>Contact page {{ namer }}</div>
  </div>
</template>

<script>
export default {
  name: 'ConactComponent',
  
  data() {
    return { namer: 'Mohamed' }
  },
  created() {},
  mounted() {
    this.getShitDone()
    console.log('ready')
  },
  asyncData() {},
  async fetch() {},
  methods: {
    async getShitDone() {
      await console.log('Am ready two')
    },
  },
}
</script>

<style></style>

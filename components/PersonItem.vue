<template>
  <div>
    <div v-if="myId">
      <h1>{{ myId.userId }}</h1>
      <h2>{{ myId.title }}</h2>
      <h3>{{ myId.completed }}</h3>
      <h3>{{ myId.id }}</h3>
    </div>
  </div>
</template>
<script lang="ts">

export default {
  props: {
    myId:[],
  },
  watch: {
    myId() {
      console.log('UPDATED')
    },
  },
}
</script>

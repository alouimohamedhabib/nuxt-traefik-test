<template>
  <div>
    ((((( {{ xDaa && xDaa.length }}
  </div>
</template>

<script>
import axios from 'axios'
export default {
//   data() {
//     return {
//       xDaa: null,
//     }
//   },
mixins: [],
  async asyncData() {
    const res = await axios.get('https://jsonplaceholder.typicode.com/todos')
    const zoom = res.data;
    // eslint-disable-next-line no-console
    console.log('P2 COMPONENT');
    return { xDaa: zoom }
  },
}
</script>

<template>
  <hello-world />
</template>

<script>
  import Calendar from '../components/Calendar'

  export default {
    data: () => ({ drawer: null }),
    
    name: 'Home',

    components: {
      Calendar,
    },
  }
</script>

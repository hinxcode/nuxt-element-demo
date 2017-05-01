<template>
  <div>
    <h1>Welcome! {{ from }}</h1>
  </div>
</template>

<script>
  const test = {
    asyncData ({ req }) {
      return {
        from: req ? 'server' : 'client'
      }
    }
  }
  export default test
</script>

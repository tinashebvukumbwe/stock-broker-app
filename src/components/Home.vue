<template>
  <div>

    <h1>Trade or view your portfolio</h1>
    <h6>save and load data</h6>
    <h6>click end day to start a new day</h6>
    <p>Your Funds: {{ funds | currency }}</p>
  </div>

</template>
<script>
  export default {
    computed: {
      funds(){
        return this.$store.getters.funds;
      }
    }
  }
</script>

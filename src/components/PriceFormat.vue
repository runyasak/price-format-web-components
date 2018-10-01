<template>
  <div>
    {{ price | numberWithCommas }}
  </div>
</template>

<script>
export default {
  name: 'PriceFormat',
  props: ['price'],
  filters: {
    numberWithCommas (number) {
      return number.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ",")
    }
  }
}
</script>


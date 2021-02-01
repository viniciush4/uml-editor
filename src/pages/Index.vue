<template>
  <q-page class="flex flex-center">
    <svg
        viewBox="0 0 100 100"
        class="full-width full-height"
    >
        <!--
        with relative unit such as percentage, the visual size
        of the square looks unchanged regardless of the viewBox
        -->
        <!-- <rect x="0" y="0" width="100%" height="100%"/> -->

        <!--
        with a large viewBox the circle looks small
        as it is using user units for the r attribute:
        4 resolved against 100 as set in the viewBox
        -->
        <circle cx="0" cy="20" r="6" fill="red"/>
    </svg>
  </q-page>
</template>

<style lang="stylus" scoped>
  svg {
    background-color: aquamarine;
  }
</style>

<script>
export default {
  name: 'PageIndex'
}
</script>

<template>
  <div :class="[$style.shape, cssClass]">
    <div>{{text}}</div>
  </div>
</template>

<script>
export default {
  name: 'BlackCircle',
  props: {
    text: String,
    cssClass: String
  }
}
</script>

<style lang="scss" module>
  .shape {
    width: 200px;
    height: 200px;
    line-height: 200px;
    color: white;
    font-weight: bold;

    /* Circles are black */
    background: black;

    /* This makes shape round */
    border-radius: 50%;
  }
</style>

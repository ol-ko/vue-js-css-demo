<template>
  <div class="shape">
    <div>{{text}}</div>
  </div>
</template>

<script>
export default {
  name: 'RedRombus',
  props: {
    text: String
  }
}
</script>

<style lang="scss" scoped>
  .shape {
    width: 200px;
    height: 200px;
    line-height: 200px;
    color: white;
    font-weight: bold;

    /* Rombuses are red */
    background: red;

    /* The following makes the shape a rombus */
    transform: rotate(45deg);

    div {
      transform: rotate(-45deg);
    }
  }
</style>

<template>
  <div>
    <button type="button" class="btn btn-secondary" :style="buttonStyle">{{buttonText}}</button>
  </div>
</template>

<script>
export default {
  name: 'ButtonVariable',
  props: {
    buttonText: {
      type: String,
      default: null
    },
    buttonStyle: {
      type: String,
      default: null
    }
  }
}
</script>
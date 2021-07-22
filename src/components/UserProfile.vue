<template>
  <div class="user-container">
    <div>
      User
    </div>
    <div class="user-description">
      <slot name="username"></slot>
      <div class="time">
        <slot name="time"></slot>
        <slot name="karma"></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    info: Object
  }
}
</script>

<style scoped>
.user-container {
  display: flex;
  align-items: center;
  padding:0.5rem;
}
.user-description {
  padding-left: 8px;
}
.time {
  font-size: 0.7rem;
}
</style>
<template>
  <button @click="openNotifications()">
    <img
      :src="require('~/assets/img/notification.svg')"
      alt="nav-logo"
    >
    <div class="messages-count">
      <span class="count-number">
        {{ countNumber }}
      </span>
    </div>
  </button>
</template>

<script>
  export default {
    data() {
      return {
        countNumber: 2
      }
    },
    methods: {
      openNotifications() {
        console.log('show notifications')
      }
    }
  }
</script>

<template>
  <a-result title="Скоро тут будут твои маршруты">
    <template #extra>
      <h3>Хочешь видеть маршрут на весь день замеров?</h3>
      <a-button type="primary" @click="openNotification">
        Да, хочу
      </a-button>
    </template>
  </a-result>
</template>

<script>
export default {
  methods: {
    openNotification() {
      this.$notification.open({
        message: 'Ваш голос учтён!',
      });
    },
  },
};
</script>

<style scoped>

</style>
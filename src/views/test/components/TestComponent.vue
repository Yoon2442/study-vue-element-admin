<template>
  <img :src="avatar + '?imageView2/1/w/160/h/160'" class="user-avatar">
</template>
<script>
import { mapGetters } from 'vuex'

export default {
  computed: {
    ...mapGetters([
      'name',
      'avatar',
      'roles'
    ])
  }
}
</script>
<style lang="scss" scoped>
.user-avatar {
  cursor: pointer;
  width: 40px;
  height: 40px;
  border-radius: 10px;
}
</style>

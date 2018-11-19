<template>
  <div class="people-list" id="people-list">
    <div class="search">
      <input type="text" placeholder="search" />
      <i class="fa fa-search"></i>
    </div>
    <ul class="list">
      <contact-item v-for="item in 10" :key="item.id"></contact-item>
    </ul>
  </div>
</template>

<script>
import contactItem from './contactItem'
export default {
  name: "contactList",
  components: { contactItem }
}
</script>

<style scoped>

</style>

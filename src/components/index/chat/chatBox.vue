<template>
  <div class="chat">

    <div class="chat-header clearfix">
      <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/195612/chat_avatar_01_green.jpg" alt="avatar" />

      <div class="chat-about">
        <div class="chat-with">Chat with Vincent Porter</div>
        <div class="chat-num-messages">already 1 902 messages</div>
      </div>
      <i class="fa fa-star"></i>
    </div>

    <div class="chat-history">
      <ul>
        <message-item v-for="item in 6" :key="item.id"></message-item>
      </ul>
    </div>

    <create-message-box></create-message-box>
  </div>
</template>

<script>
import messageItem from './messageItem'
import createMessageBox from './createMessageBox'
export default {
  name: "chatBox",
  components: { createMessageBox, messageItem }
}
</script>

<style scoped>

</style>

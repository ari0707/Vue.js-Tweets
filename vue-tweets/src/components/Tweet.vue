<template>


    <div class="tweet">
        <ProfileImage :image="user.image" />

        <div class="body">
          <div class="top">
            <User :userData="user" />
            <TimeStamp :timestamp="timestamp" />
          </div>
    
          <Message :message="message" />
          <Actions />
        </div>
    
        <i class="fas fa-ellipsis-h"></i>
      </div>
    </template>

<script>

import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import TimeStamp from './TimeStamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

export default {
    name: "Tweet",
    components: {
        ProfileImage, 
        User, 
        TimeStamp, 
        Message, 
        Actions 
    },
    props: [
        "user",
        "timestamp", 
        "message", 
    ]
}
</script>
  
<style scoped>
  a {
    color: #42b983;
  }
</style>
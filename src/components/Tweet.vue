<template>
    <div class="tweet">


        <ProfileImage :image="tweet.user.image" />

        <div class="body">
            <div class="top">

                <User :name="tweet.user.name" :handle="tweet.user.handle" />

                <Timestamp :timestamp="tweet.timestamp" />
            </div>

            <Message :message="tweet.message" />

            <Actions />

        </div>

        <i class="fas fa-ellipsis-h"></i>
    </div>
    
</template>


<script setup>

import { defineProps } from 'vue'
import Actions from './Actions.vue'
import Timestamp from './Timestamp.vue'
import User from './User.vue'
import Message from './Message.vue';
import ProfileImage from './ProfileImage.vue';

const props = defineProps (['tweet']);

</script>
  
<style scoped>
a {
    color: #42b983;
}
</style>
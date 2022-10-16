import { defineProps } from 'vue';
<template>
    <div class="tweet">
        <ProfileImage />
        <div class="body">
            <div class="top">
                <span class="user">
                    <User />
                </span>
                <Timestamp />
            </div>

            <Message />

            <Actions />
        </div>

        <i class="fas fa-ellipsis-h"></i>

    </div>
</template>
  

<script setup>

import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';


import {defineProps} from 'vue'
const props = defineProps(["tweet"]);

</script>


<style scoped>
a {
    color: #42b983;
}
</style>
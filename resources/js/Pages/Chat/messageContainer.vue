<template>
    <div class="h-96 w-full">
        <div class="h-full p-2 flex flex-col-reverse overflow-scroll">
            <div v-for="(message, index) in messages" :key="index">
                 <detail-message :message="message" />
            </div>
        </div>
    </div>
</template>

<script>
import detailMessage from './detailMessage.vue'

export default {
  components: { detailMessage },
    
    props: ['messages'],
  
}
</script>
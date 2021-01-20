<template>
    <div class="online-status">
        <div v-if="online" class="online">
            <span class="light"></span>
            <p>A staff member is online</p>
        </div>
        <div v-if="!online" class="offline">
            <span class="light"></span>
            <p>A staff member is not online</p>
        </div>
    </div>
</template>

<script>
export default {

    props: ['status'],

    data(){
        return{
            //online: true,
        }
    },

    computed: {
        online(){
            return this.status == 'online';
        }
    }
}
</script>

<style scoped>

</style>
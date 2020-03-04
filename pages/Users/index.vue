<template>
    <div>
        <input type="text" v-model ="userId">
     <button @click="OnLoadUser"> Load User </button>
     </div>
</template>

<script>
export default {
    data () {
        return {
            userId : ''
        }
    },
    methods: {
        OnLoadUser() {
            this.$router.push('/users/'+ this.userId)
        }
    }
}
</script>
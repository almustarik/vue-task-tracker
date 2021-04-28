<template>
    <button @click="onClick()"
    :style="{ background: color }"
    class="btn">{{ text }}</button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        text: String,
        color: String,
    },
    methods: {
        onClick() {
            // this.$$emit('delete-task', id)
            this.$emit('btn-click')
        }
    }
}
</script>
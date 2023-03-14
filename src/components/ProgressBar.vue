<template>
    <div :style="{ width: progressBarWidth }" id="progress-bar-full"></div>
</template>

<script>
    export default {
        props: {
            current: {
                type: Number,
                required: true
            }
        },

        computed: {
            progressBarWidth() {
                return (this.current + 1) * 10 + '%';
            }
        },
    }
</script>

<style>
    #progress-bar-full {
    width: 100px;
    height: 34px;
    border-radius: 20px;
    box-shadow: rgba(0, 0, 0, 0.4) 0px 2px 4px, rgba(0, 0, 0, 0.3) 0px 7px 13px -3px, rgba(0, 0, 0, 0.2) 0px -3px 0px inset;
    background-color: #ffd60a;
    width: 0%;
}
</style>
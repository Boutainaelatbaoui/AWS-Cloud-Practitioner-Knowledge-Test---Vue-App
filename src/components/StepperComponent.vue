<script>
    export default {
        props: {
            step: {
                type: Number,
                required: true
            }
        },

        computed : {
            stepperProgress() {
                return ( 100 / 3 ) * (this.step - 1) + '%';
            }
        }
    }
</script>

<template>
    <div class="wrapper-stepper">
        <div class="stepper">
            <div class="stepper-progress">
                <div class="stepper-progress-bar" :style="'width:' + stepperProgress">
                </div>
            </div>

            <div class="stepper-item" :class="{'current': step == item, 'success': step > item}" v-for="item in 3" :key="item">
                <div class="stepper-item-counter">
                    <i class="bi bi-check-lg icon"></i>
                    <span class="number">
                        {{ item }}
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
    
</style>
<template>
    <h1>Confetti</h1>
</template>

<script>
import Vue from 'vue'
import VueConfetti from 'vue-confetti'

Vue.use(VueConfetti)

export default {
    mounted: function () {
        this.$confetti.start({
            shape: 'circle',
            colors: ['DodgerBlue', 'OliveDrab', 'Gold', 'pink', 'SlateBlue', 'lightblue', 'Violet', 'PaleGreen', 'SteelBlue', 'SandyBrown', 'Chocolate', 'Crimson']
        })
        setTimeout(() => {
            this.$confetti.stop()
        }, 4000)
    },
    methods: {}
}
</script>

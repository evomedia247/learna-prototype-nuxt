<template>
<div class="container-fluid rouge-bg text-center">
    <h1 class="title-font py-85 text-white">Our MBA Courses</h1>
        <!-- <client-only>
        <Lottie
            className="animation"
            renderer="svg"
            :loop="true"
            :autoplay="true"
            :animationData=Banner
            @getLottieInstance=getLottieInstance
            @onEnterFrame=onEnterFrame
            @onComplete=onComplete
            @onLoopComplete=onLoopComplete
        />
    </client-only> -->
</div>

</template>
<script>
import Lottie from 'vue-lottie-web'
import Banner from 'assets/test.json'
export default {
    components: {
        Lottie
    },
    data() {
        return {
            Banner,
            lottieInstance: '',
        };
    },
    methods: {
        getLottieInstance(lottieInstance) {
            this.lottieInstance = lottieInstance;
            // console.log(lottieInstance)
        },
        lottiePlay() {
            this.lottieInstance && this.lottieInstance.play();
        },
        lottieRePlay() {
            this.lottieInstance && this.lottieInstance.stop();
            setTimeout(() => {
                this.lottieInstance.play();
            });
        },
        lottiePause() {
            this.lottieInstance && this.lottieInstance.pause();
        },
        lottieStop() {
            this.lottieInstance && this.lottieInstance.stop();
        },
        onComplete(e) {
            // console.log('onComplete', e);
        },
        onLoopComplete(e) {
            // console.log('onLoopComplete', e);
        },
        onEnterFrame(e) {
            // console.log('onEnterFrame', e);
        }
    }
}
</script>
<style scoped>
h1 {
    font-size: 4em;
}

.bgimage {
    width: 100%;
    height: 250px;
    background: linear-gradient(40deg, rgba(242, 1, 98, 1) 0%, rgba(197, 22, 77, 1) 100%);
    background: url("../assets/banner.jpg");
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
    color: #3b335d !important;
}

.rouge-bg {
    background: #B93E73;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to bottom, #B93E73, #F0508A);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to bottom, #B93E73, #F0508A); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

.bgimage h5 {
    text-shadow: 2px 2px #333;
}
</style>
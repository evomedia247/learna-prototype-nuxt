<template>
   <div class="container-fluid py-85 sea-blue-bg text-white">
       
        <div class="container">
            
        <div class="row mb-5">
            <div class="col text-center fade-in3">
                <h4 class="section-title aos-init aos-animate title-font" data-aos-duration="500" data-aos="fade-down" data-aos-delay="0">Why study with Learna</h4>
                <h3 class="subheading aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="250">We are exceptionally proud of the work that we do, our postgraduate courses provide students and professionals with exceptional, flexible and affordable, online education.</h3>
            </div>
        </div>
        <div class="row fade-in3 mb-2">
            <div class="col-md-4 text-center aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="250">
                <div class="mx-auto mb-2" style="width: 100px; height 100px">
                    <client-only>
                        <Lottie
                        className="animation"
                        renderer="svg"
                        :loop="true"
                        :autoplay="true"
                        :animationData=WhyValue
                        @getLottieInstance=getLottieInstance
                        @onEnterFrame=onEnterFrame
                        @onComplete=onComplete
                        @onLoopComplete=onLoopComplete
                    />
                    </client-only>
                </div>
                <h4 class="subheading title-font">Affordable Education</h4>
                <p>Our programmes provide the highest quality education at amazingly low costs.</p>
        </div>
            <div class="col-md-4 text-center aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="500">
                <div class="mx-auto mb-2" style="width: 100px; height 100px">
                    <client-only>
                    <Lottie
                        className="animation"
                        renderer="svg"
                        :loop="true"
                        :autoplay="true"
                        :animationData=WhyOnline
                        @getLottieInstance=getLottieInstance
                        @onEnterFrame=onEnterFrame
                        @onComplete=onComplete
                        @onLoopComplete=onLoopComplete
                    />
                    </client-only>
                </div>
                <h4 class="subheading title-font">Fully Online</h4>
            <p> No fixed study times mean you can log in and learn whenever suits you.</p>
        </div>
            <div class="col-md-4 text-center aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="750">
                <div class="mx-auto mb-2" style="width: 100px; height 100px">
                    <client-only>
                    <Lottie
                        className="animation"
                        renderer="svg"
                        :loop="true"
                        :autoplay="true"
                        :animationData=WhyGrad
                        @getLottieInstance=getLottieInstance
                        @onEnterFrame=onEnterFrame
                        @onComplete=onComplete
                        @onLoopComplete=onLoopComplete
                    />
                    </client-only>
                </div>
                <h4 class="subheading title-font">Graduate Faster</h4>
            <p>Get a postgraduate qualification in just 1 calendar year instead of 2 academic years.</p>
            </div>
            <div class="col-md-4 text-center aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="250">
                <div class="mx-auto mb-2" style="width: 100px; height 100px">
                    <client-only>
                    <Lottie
                        className="animation"
                        renderer="svg"
                        :loop="true"
                        :autoplay="true"
                        :animationData=WhyExperts
                        @getLottieInstance=getLottieInstance
                        @onEnterFrame=onEnterFrame
                        @onComplete=onComplete
                        @onLoopComplete=onLoopComplete
                    />
                    </client-only>
                </div>
                <h4 class="subheading title-font">Learn with Experts</h4>
            <p>Our tutors are selected from a global pool of experts to provide award winning tuition.</p>
            </div>
            <div class="col-md-4 text-center aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="500">
                <div class="mx-auto mb-2" style="width: 100px; height 100px">
                    <client-only>
                    <Lottie
                        className="animation"
                        renderer="svg"
                        :loop="true"
                        :autoplay="true"
                        :animationData=WhyEthical
                        @getLottieInstance=getLottieInstance
                        @onEnterFrame=onEnterFrame
                        @onComplete=onComplete
                        @onLoopComplete=onLoopComplete
                    />
                    </client-only>
                </div>
                <h4 class="subheading title-font">Ethical Learning</h4>
            <p>Studying online produces 90% fewer emissions than campus learning.</p>
        </div>
            <div class="col-md-4 text-center aos-init aos-animate" data-aos-duration="500" data-aos="fade-down" data-aos-delay="750">
                <div class="mx-auto mb-2" style="width: 100px; height 100px">
                    <client-only>
                    <Lottie
                        className="animation"
                        renderer="svg"
                        :loop="true"
                        :autoplay="true"
                        :animationData=WhyConn
                        @getLottieInstance=getLottieInstance
                        @onEnterFrame=onEnterFrame
                        @onComplete=onComplete
                        @onLoopComplete=onLoopComplete
                    />
                    </client-only>
                </div>
                <h4 class="subheading title-font">Make Connections</h4>
            <p>Connect with students based all around the world to help your career prosper.</p>
            </div>
        </div>
        </div>
    </div>
</template>
<style scoped>

    .sea-blue-bg {
        background: #B93E73;  /* fallback for old browsers */
        background: -webkit-linear-gradient(to bottom, #B93E73, #F0508A);  /* Chrome 10-25, Safari 5.1-6 */
        background: linear-gradient(to bottom, #B93E73, #F0508A); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    }

    p {
        color: white;
    }
</style>
<script>
import Lottie from 'vue-lottie-web'
import lottieData from 'assets/26893-rocket.json'
import WhyExperts from 'assets/why-experts.json'
import WhyEthical from 'assets/why-ethical.json'
import WhyOnline from 'assets/why-online.json'
import WhyValue from 'assets/why-value.json'
import WhyGrad from 'assets/why-grad.json'
import WhyConn from 'assets/why-conn.json'

export default {
    components: {
        Lottie
    },
    data() {
        return {
            lottieData,
            WhyExperts,
            WhyEthical,
            WhyOnline,
            WhyValue,
            WhyGrad,
            WhyConn,
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
};
</script>
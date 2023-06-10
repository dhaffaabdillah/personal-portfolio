<template>
    <!-- eslint-disable-next-line max-len -->
    <!-- Section - Services -->
    <section class="lui-section lui-gradient-bottom" id="services-section">

        <!-- Heading -->
        <div class="lui-heading">
            <div class="container">

                        <div class="m-titles align-center">
                            <h2 class="m-title splitting-text-anim-1 scroll-animate" data-splitting="words" data-animate="active">
                                <span> What I Do </span>
                            </h2>
                            <!-- <div class="m-subtitle splitting-text-anim-1 scroll-animate" data-splitting="words" data-animate="active">
                                <span> my <b>Services</b> </span>
                            </div> -->
                        </div>

            </div>
        </div>

        <!-- Services -->
        <div class="v-line v-line-right">
            <div class="container">

                    <div class="swiper-container js-services scrolla-element-anim-1 scroll-animate" data-animate="active">
                        <div class="swiper-wrapper">
                            <!-- looping data -->
                            <div class="swiper-slide" v-for="item in listServices" :key="item.id">
                                <div class="services-item">
                                    <div class="lui-subtitle">
                                        <span> {{ item.serviceSubTitle}} </span>
                                    </div>
                                    <div class="icon"></div>
                                    <h5 class="lui-title">
                                        <span> {{ item.serviceTitle}} </span>
                                    </h5>
                                    <div class="lui-text">
                                        <div> {{ item.serviceDescription}} </div>
                                    </div>
                                    <a href="#pricing-section" class="lnk"> See Pricing </a>
                                    <div class="image" style="background-image: url(assets/images/pat-2.png);"></div>
                                </div>
                            </div>
                        </div>
                        <div class="swiper-pagination"></div>
                    </div>

                    <div class="lui-bgtitle">
                        <span> Services </span>
                    </div>

                </div>
            </div>

    </section>
</template>
<script>
export default {
    name: "ServicesComponents",
    data() {
        return {
            listServices: [
                {
                    'id' : 1,
                    'serviceTitle' : "Web Development",
                    'serviceSubTitle' : "Web Development",
                    'serviceDescription' : "Website development is now very much needed, especially people who are starting businesses and companies."
                },
                {
                    'id' : 2,
                    'serviceTitle' : "Mobile Development",
                    'serviceSubTitle' : "Android & iOS",
                    'serviceDescription' : "Design Software applications to run on mobile devices. Modern and mobile-ready application that will help you reach all of your marketing."
                },
                {
                    'id' : 3,
                    'serviceTitle' : "Video Editing",
                    'serviceSubTitle' : "Premiere Pro, After Effects",
                    'serviceDescription' : "Video editing is one of my hobby, doing with enjoy."
                },
            ]
        }
    }, 
    methods: {
        getServices() {
            this.listServices
        }
    },
}
</script>
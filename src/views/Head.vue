<template>

    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <Headsection/>

</template>

<script>
// @ is an alias to /src
import Headsection from '@/components/navbar/Headsection.vue'

export default {
  name: 'Head',
  components: {
    Headsection
  },

  mounted(){

        // Category Owl Carousel
    const objowlcarousel = $('.owl-carousel-category');
    if (objowlcarousel.length > 0) {
        objowlcarousel.owlCarousel({
            responsive: {
                0: {
                    items: 3,
                },
                600: {
                    items: 4,
                },
                1000: {
                    items: 6,
                },
                1200: {
                    items: 8,
                },
            },
            loop: true,
            lazyLoad: true,
            autoplay: true,
            dots: false,
            autoplaySpeed: 1000,
            autoplayTimeout: 2000,
            autoplayHoverPause: true,
            nav: true,
            navText: ["<i class='fa fa-chevron-left'></i>", "<i class='fa fa-chevron-right'></i>"],
        });
    }

      // Homepage Owl Carousel  
    var fiveobjowlcarousel = $(".owl-carousel-four");
    if (fiveobjowlcarousel.length > 0) {
        fiveobjowlcarousel.owlCarousel({
            responsive: {
                0: {
                    items: 1,
                },
                600: {
                    items: 2,
                },
                1000: {
                    items: 4,
                },
                1200: {
                    items: 4,
                },
            },

            lazyLoad: true,
            pagination: false,
            loop: true,
            dots: false,
            autoPlay: 2000,
            nav: true,
            stopOnHover: true,
            navText: ["<i class='icofont-thin-left'></i>", "<i class='icofont-thin-right'></i>"]
        });
    }

    // Owl Carousel Five
    var fiveobjowlcarousel = $(".owl-carousel-five");
    if (fiveobjowlcarousel.length > 0) {
        fiveobjowlcarousel.owlCarousel({
            responsive: {
                0: {
                    items: 2,
                },
                600: {
                    items: 3,
                },
                1000: {
                    items: 4,
                },
                1200: {
                    items: 5,
                },
            },
            lazyLoad: true,
            pagination: false,
            loop: true,
            dots: false,
            autoPlay: 2000,
            nav: true,
            stopOnHover: true,
            navText: ["<i class='icofont-thin-left'></i>", "<i class='icofont-thin-right'></i>"]
        });
    }

    // Homepage Ad Owl Carousel
    const mainslider = $('.homepage-ad');
    if (mainslider.length > 0) {
        mainslider.owlCarousel({
            responsive: {
                0: {
                    items: 2,
                },
                764: {
                    items: 2,
                },
                765: {
                    items: 1,
                },
                1200: {
                    items: 1,
                },
            },
            lazyLoad: true,
            loop: true,
            autoplay: true,
            autoplaySpeed: 1000,
            dots: false,
            autoplayTimeout: 2000,
            nav: true,
            navText: ["<i class='fa fa-chevron-left'></i>", "<i class='fa fa-chevron-right'></i>"],
            autoplayHoverPause: true,
        });
    }

  },
 
}
</script>

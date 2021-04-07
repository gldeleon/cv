<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="100%"
      img-height="100%"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption=""
        text=""
        img-src="https://picsum.photos/1920/1005/?image=56"
      ></b-carousel-slide>

      <b-carousel-slide
        caption=""
        text=""
        img-src="https://picsum.photos/1920/1005/?image=57"
      ></b-carousel-slide>

      <b-carousel-slide
        caption=""
        text=""
        img-src="https://picsum.photos/1920/1005/?image=58"
      ></b-carousel-slide>

      <b-carousel-slide
        caption=""
        text=""
        img-src="https://picsum.photos/1920/1005/?image=59"
      ></b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
  export default {
    name: 'Carousel',
    data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart() {
        this.sliding = true
      },
      onSlideEnd() {
        this.sliding = false
      }
    }
  }
</script>
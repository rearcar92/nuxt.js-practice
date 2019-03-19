<template>
  <div>
    <main-carousel>
      <a slot="link" href="http://twinkring.com/">
        <b-carousel-slide caption="" slot="image" img-src="http://twinkring.com/2019/02/star/star_fullbanner.jpg" />
      </a>
      <a slot="link" href="http://thechanran.com/">
        <b-carousel-slide caption="" slot="image" img-src="http://twinkring.com/2019/03/bk/bk_fullbanner.jpg" />
      </a>  
    </main-carousel>
  </div>
</template>

<script>
import mainCarousel from '~/components/common/Carousel.vue';
export default {
  components: {
    mainCarousel
  }
}
</script>

<style>

</style>

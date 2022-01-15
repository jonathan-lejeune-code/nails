<template>
  <div class="home">
    <Gallery v-bind:images="images" />
  </div>
</template>

<script>
import Gallery from '../components/Gallery'
export default {
  name: 'PhotosPage',
  components: {
    Gallery,
  },
  data() {
    return {
      dialog: false,
      images: [
        { id: 1, imgSrc: require('@/assets/nails1.jpg') },
        { id: 2, imgSrc: require('@/assets/nails2.jpg') },
        { id: 3, imgSrc: require('@/assets/nails3.jpeg') },
        { id: 4, imgSrc: require('@/assets/nails4.webp') },
        { id: 5, imgSrc: require('@/assets/nails5.jpg') },
        { id: 6, imgSrc: require('@/assets/nails6.jpeg') },
        { id: 7, imgSrc: require('@/assets/nails7.jpg') },
        { id: 8, imgSrc: require('@/assets/nails8.jpg') },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
h2 {
  background-color: orange;
  border-radius: 10px;
  font-size: 50px;
  margin: 10px auto;
}
</style>

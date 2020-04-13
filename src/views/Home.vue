<template>
  <div>
    <div id="banner">
      <b-carousel
        id="carousel-1"
        v-model="slide"
        :interval="4000"
        indicators
        background="#ababab"
        img-width="1024"
        img-height="300"
        style="text-shadow: 1px 1px 2px #333;"
      >
        <!-- Slide with blank fluid image to maintain slide aspect ratio -->
        <b-carousel-slide img-blank img-alt="Blank image">
          <template v-slot:img>
            <img
              class="d-block img-fluid w-100"
              width="1024"
              height="480"
              src="../assets/banner.jpg"
              alt="image slot"
            />
          </template>
        </b-carousel-slide>
        <b-carousel-slide img-blank img-alt="Blank image">
          <template v-slot:img>
            <img
              class="d-block img-fluid w-100"
              width="1024"
              height="480"
              src="../assets/banner.jpg"
              alt="image slot"
            />
          </template>
        </b-carousel-slide>
      </b-carousel>
    </div>
    <section>
      <b-container class="pt-4">
        <b-row>
          <mood></mood>
          <traveling></traveling>
        </b-row>
      </b-container>
    </section>
    <featured></featured>
  </div>
</template>

<script>
import Mood from "../components/home/Mood.vue";
import Traveling from "../components/home/Traveling.vue";
import Featured from "../components/home/Featured";
export default {
  name: "Home",
  components: { mood: Mood, traveling: Traveling, featured: Featured }
};
</script>

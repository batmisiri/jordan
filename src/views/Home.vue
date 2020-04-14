<template>
  <div style ="position: relative;">
    <div id="banner">
      <b-carousel
      
        id="carousel-1"
        :interval="4000"
        indicators
        background="#ababab"
        img-width="1024"
        img-height="300"
        style="text-shadow: 1px 1px 2px #333;"

      >
        <!-- Slide with blank fluid image to maintain slide aspect ratio -->
       <bannerContent svg_banner = "banner1.png"/>
       <bannerContent svg_banner = "banner2.png"/>
        <bannerContent svg_banner = "banner1.png"/>
       <bannerContent svg_banner = "banner2.png"/>
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
    <section>
      <premium-experience></premium-experience>
    </section>
    <section>
      <travellers-use></travellers-use>
    </section>
    <section>
      <featured-in></featured-in>
    </section>
  </div>
</template>

<script>
import BannerContent from "../components/home/BannerContent.vue";
import Mood from "../components/home/Mood.vue";
import Traveling from "../components/home/Traveling.vue";
import Featured from "../components/home/Featured";
import PremiumExperience from "../components/home/PremiumExperience";
import TravellersUse from "../components/home/TravellersUse";
import FeaturedIn from "../components/home/FeaturedIn";
export default {
  name: "Home",
  components: {
    bannerContent: BannerContent,
    mood: Mood,
    traveling: Traveling,
    featured: Featured,
    "premium-experience": PremiumExperience,
    "travellers-use": TravellersUse,
    "featured-in": FeaturedIn
  }
};
</script>

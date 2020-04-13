<template>
  <section class="text-left">
    <b-container>
      <b-row>
        <b-col cols="10"><h1 class="heading">Featured Programs</h1></b-col>
        <b-col cols="2 text-right"></b-col>
      </b-row>
    </b-container>
    <div class="featured-wrap">
      <b-container>
        <b-row>
          <b-col>
            <carousel :items="4" :nav="true" :dots="false" :margin="20">
              <div class="featured-box">
                <h2>Weekend In Joradn</h2>
                <figure>
                  <img src="../../assets/0015.png" alt="" />
                  <figcaption>
                    <book-now-btn text="Book Now"></book-now-btn>
                  </figcaption>
                </figure>
              </div>
              <div class="featured-box">
                <h2>Weekend In Joradn</h2>
                <figure>
                  <img src="../../assets/0016.png" alt="" />
                  <figcaption>
                    <book-now-btn text="Book Now"></book-now-btn>
                  </figcaption>
                </figure>
              </div>
              <div class="featured-box">
                <h2>Weekend In Joradn</h2>
                <figure>
                  <img src="../../assets/0017.png" alt="" />
                  <figcaption>
                    <book-now-btn text="Book Now"></book-now-btn>
                  </figcaption>
                </figure>
              </div>
              <div class="featured-box">
                <h2>Weekend In Joradn</h2>
                <figure>
                  <img src="../../assets/0018.png" alt="" />
                  <figcaption>
                    <book-now-btn text="Book Now"></book-now-btn>
                  </figcaption>
                </figure>
              </div>
              <div class="featured-box">
                <h2>Weekend In Joradn</h2>
                <figure>
                  <img src="../../assets/0015.png" alt="" />
                  <figcaption>
                    <book-now-btn text="Book Now"></book-now-btn>
                  </figcaption>
                </figure>
              </div>
              <div class="featured-box">
                <h2>Weekend In Joradn</h2>
                <figure>
                  <img src="../../assets/0015.png" alt="" />
                  <figcaption>
                    <book-now-btn text="Book Now"></book-now-btn>
                  </figcaption>
                </figure>
              </div>
            </carousel>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </section>
</template>

<script>
import carousel from "vue-owl-carousel";
import Button from "../common/Button";

export default {
  components: { carousel, "book-now-btn": Button }
};
</script>

<style lang="scss">
.featured-box {
  position: relative;
  padding: 20px 0;
  h2 {
    font-size: 16px;
    text-transform: uppercase;
    color: #000;
    text-align: center;
    font-weight: bold;
  }
  figure {
    position: relative;
    figcaption {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      padding: 20px;
      a {
        right: 20px;
        bottom: -30px;
        position: absolute;
      }
    }
  }
}
</style>

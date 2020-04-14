<template>
    <b-carousel-slide img-blank img-alt="Blank image" class = "banner-carousel">
        <template v-slot:img>
        <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            :src="require(`../../assets/png/${svg_banner}`)"
            alt="image slot"
        />
        <p class = "banner-text">Book your authentic trip, <br/>get the unique experience.</p>
        <img src = "../../assets/png/booktrip.png" class = "book-trip-svg"/>
        <p class = "book-trip-text"> BOOK A TRIP </p>
        <img src = "../../assets/png/rentcar.png" class = "rent-car-svg" />
        <p class = "rent-car-text"> RENT A CAR </p>
        <img src = "../../assets/png/map.png" class = "map-png"/>
        <p class = "map-text1">MOST POPULAR</p>
        <p class = "map-text2">Al- Khazneh, Petra</p>
        <p class = "map-text3">DISCOVER DESTINATION</p>
        <img src = "../../assets/png/line.png" class = "map-line-png"/>
        <img src = "../../assets/png/next.png" class = "map-next-png"/>
        </template>
    </b-carousel-slide>
</template>

<script>
export default {
    name: "BannerContent",
    props:{
      svg_banner: String
    }
}
</script>
<style>
@font-face {
  font-family: Poppins;
  src: url("../../assets/font/Poppins-Regular.ttf");
}
.banner-carousel{
  position: relative;
}

.map-png{
  position: absolute;
  left: 75%;
  top: 64.13%;
}
.map-line-png{
  position: absolute;
  left: 80%;
  top: 78%;
}
.map-next-png{
  position: absolute;
  left: 92%;
  top: 77%;  
}
.map-text3{
  position: absolute;
  left:83%;
  top: 77%;
  font-family: Poppins;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 21px;
  color: #FFFFFF;
}

.map-text2{
  position: absolute;
  left:80%;
  top: 70%;
  font-family: Poppins;
  font-style: normal;
  font-weight: 300;
  font-size: 28px;
  line-height: 42px;
  color: #FFFFFF;
}

.map-text1{
  position: absolute;
  left: 80%;
  top: 66%;
  font-family: Poppins;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 24px;
  /* identical to box height */
  color: #FFFFFF;
}
.banner-text{
  position: absolute;
  left: 8.68%;

  top: 8.54%;
  font-family: Poppins;
  font-style: normal;
  font-weight: bold;
  font-size: 58px;
  line-height: 87px;
  color: #FFFFFF;
}
.book-trip-text{
  position: absolute;
  left: 11.6%;
  top: 84.13%;

  font-family: Poppins;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 24px;
  /* identical to box height */
  color: #FFFFFF;
}
.book-trip-svg{
  position: absolute;
  left: 9.1%;
  top: 84.24%;
}
.rent-car-text{
  position: absolute;
  left: 23.61%;
  top: 84.13%;

  font-family: Poppins;
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;
  /* identical to box height */
  color: #FFFFFF;
}
.rent-car-svg{
  position: absolute;
  left: 21.11%;
  top: 84.11%;
}
</style>
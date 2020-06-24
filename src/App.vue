<template>
  <div id="app">
    <img width="25%" :src="logo[0].src">
    <HelloWorld :msg="message"/>
    <!-- SINGLE SELECTION -->
    <ImageSelect :dataImages="dataImages" @onselectimage="onSelectImage"></ImageSelect>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import ImageSelect from "./components/ImageSelect.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    ImageSelect
  },
  data: function() {
    return {
      logo: [
        {
          id: 1,
          src:
            "https://i.pinimg.com/originals/0c/67/5a/0c675a8e1061478d2b7b21b330093444.gif"
        }
      ],
      message: "Hello! This should allow image based selection!",
      dataImages: [
        {
          id: 1,
          src:
            "https://cdn.icon-icons.com/icons2/2416/PNG/512/circle_doodle_heart_plate_shape_valentine_favorite_button_icon_146721.png",
          alt: "Love things and love your self!"
        },
        {
          id: 2,
          src:
            "https://cdn.icon-icons.com/icons2/2416/PNG/512/heart_list_task_to_do_icon_146658.png",
          alt: "Keep bullet journaling!"
        },
        {
          id: 3,
          src:
            "https://cdn.icon-icons.com/icons2/2416/PNG/512/alcohol_bar_bottle_champagne_drink_romantic_toast_icon_146713.png",
          alt: "Take it easy ❦"
        },
        {
          id: 4,
          src:
            "https://cdn.icon-icons.com/icons2/2416/PNG/512/draw_edit_heart_line_pen_writing_icon_146731.png",
          alt: "Always write things down."
        }
      ]
    };
  },
  methods: {
    onSelectImage: function(image) {
      this.message = "You clicked image " + image.id + "! <br>" + image.alt;
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.select-image__thumbnail {
  max-width: 9em;
}
</style>

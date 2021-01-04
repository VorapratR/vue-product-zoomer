<template>
  <client-only>
    <!-- <div style="height: 100vh">
      <ProductZoomer
        :base-images="images"
        :base-zoomer-options="zoomerOptions"
      />
    </div> -->
    <div style="height: 100vh">
      <ProductZoomer
        :base-images="images"
        :base-zoomer-options="zoomerOptions2"
      />
    </div>
  </client-only>
</template>

<script>
export default {
  data() {
    return {
      images: {
        thumbs: [
          {
            id: 1,
            url:
              "https://www.flaticon.com/svg/static/icons/svg/3930/3930499.svg",
          },
          {
            id: 2,
            url:
              "https://seller-api.d3-dots.com/productImage/200208060221796.jpg",
          },
        ],
        normal_size: [
          {
            id: 1,
            url:
              "https://www.flaticon.com/svg/static/icons/svg/3930/3930499.svg",
          },
          {
            id: 2,
            url:
              "https://seller-api.d3-dots.com/productImage/200208060221796.jpg",
          },
        ],
      },
      zoomerOptions: {
        zoomFactor: 3,
        pane: "container-round",
        hoverDelay: 300,
        namespace: "zoomer-bottom",
        move_by_click: false,
        scroll_items: 4,
        choosed_thumb_border_color: "#cae724",
        scroller_position: "bottom",
        zoomer_pane_position: "right",
      },
      zoomerOptions2: {
        zoomFactor: 3,
        pane: "container-round",
        hoverDelay: 300,
        namespace: "zoomer-bottom",
        move_by_click: false,
        scroll_items: 4,
        choosed_thumb_border_color: "#cae724",
        scroller_position: "left",
        zoomer_pane_position: "right",
      },
    };
  },
};
</script>

<style scoped>
</style>

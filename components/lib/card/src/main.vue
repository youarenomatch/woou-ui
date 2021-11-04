<template>
  <div class="w-card" :style="width ? { width: width + 'px' } : {}">
    <div
      class="w-card-img"
      :style="imgHeight ? { height: imgHeight + 'px' } : {}"
    >
      <img :src="imgSrc" alt="img" />
    </div>
    <div v-if="summary" class="w-card-summary">{{ summary }}</div>
    <div v-else class="w-card-summary"><slot></slot>></div>
    <slot name="footer"></slot>
  </div>
</template>

<script>
export default {
  name: "w-card",
  props: {
    width: {
      //卡片宽度
      type: Number,
      default: 0
    },
    imgSrc: {
      //卡片的图片地址
      type: String,
      default: ""
    },
    imgHeight: {
      // 卡片的高度
      type: Number,
      default: 0
    },
    summary: {
      type: String,
      default: ""
    }
  }
};
</script>

<style lang="scss" scoped></style>

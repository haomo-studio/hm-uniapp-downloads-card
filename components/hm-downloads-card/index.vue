<template>
  <div class="hm-downloads-card">
    <div class="container">
      <div class="downloadDetail">
        <div class="downloadDetail-container">
          <text class="count">{{ options.count }}</text>
          <text class="downloads">{{ options.downloads }}</text>
        </div>
      </div>
      <image class="downloadImage" :src="options.downloadImage" />
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmDownloadsCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-downloads-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          count: '299.674',
          downloads: '下载量',
          downloadImage:
            './images/img_24402_0_0.png'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>

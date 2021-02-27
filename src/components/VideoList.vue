<template>
  <ul>
    VideoList
    <VideoListItem
      v-for="video in videos"
      v-bind:video="video"
      :key="video.etag"
    ></VideoListItem>
  </ul>
</template>

<script>
import VideoListItem from './VideoListItem'

export default {
  name: 'VideoList',
  props: { videos: Array },
  components: { VideoListItem }
}
</script>

<style></style>

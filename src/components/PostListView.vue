<template>
  <div class="post-list">
    <div v-for="post in posts" :key="post">
        <SinglePost :post="post" />
    </div>
  </div>
</template>

<script>
import { onMounted, onUnmounted, onUpdated } from 'vue'
import SinglePost from '../components/SinglePostView.vue'
export default {
    props: ['posts'],
    components: { SinglePost },
    setup(props) {
        // console.log(props.posts)
        onMounted(() => console.log("component mounted"))
        onUnmounted(() => console.log("component unmounted"))
        onUpdated(() => console.log("component updated"))
    }
}
</script>

<style>

</style>
<template>
  <div id="app">
    <h2 class="text-center text-3xl p-7">UpVote!</h2>
    <div class="flex justify-center">
      <Upvote
        :id="submissions[0].id"
        :title="submissions[0].title"
        :avatar="submissions[0].avatar"
        :description="submissions[0].description"
        :votes="submissions[0].votes"
        :submissionImage="submissions[0].submissionImage"
      />
    </div>
  </div>
</template>

<script>
import Upvote from "./components/Upvote.vue"
import { submissions } from "./data/seed"

export default {
  name: "App",
  components: {
    Upvote,
  },
  data() {
    return {
      submissions,
    }
  },
}
</script>

<style></style>
"", "title", "description", "url", "votes", "avatar", "submissionImage"

<!-- :imageUrl="submissions[0].imageUrl" -->
<!-- :url="submissions[0]" -->

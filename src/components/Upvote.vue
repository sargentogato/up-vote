<template>
  <article class="flex gap-3 border p-5 w-fit">
    <figure>
      <img class="w-[64px]" :src="submissionImage" />
    </figure>
    <div>
      <div>
        <p>
          <strong>
            <a href="#">{{ title }}</a>
            <span>{{ id }}</span>
          </strong>
          <br />
          {{ description }}
          <br />
          <small class="flex gap-3">
            Submitted by:
            <img class="w-[24px] rounded-xl" :src="avatar" />
          </small>
        </p>
      </div>
    </div>
    <div>
      <span>
        <i class="fa fa-chevron-up"></i>
        <strong>{{ votes }}</strong>
      </span>
    </div>
  </article>
</template>

<script>
export default {
  name: "Upvote",
  props: [
    "id",
    "title",
    "description",
    "url",
    "votes",
    "avatar",
    "submissionImage",
  ],
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>

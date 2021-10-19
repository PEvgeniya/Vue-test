<template>
  <v-card>
    <v-img height="75vh" :src="page_info.cat"> </v-img>
    <h1 class="font-weight-bold grey--text text--{lighten-5}">
      {{ page_info.title }}
    </h1>

    <v-card-text>
      <p class="font-weight-light">
        {{ page_info.description }}
      </p>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  name: "ListItem",
  data: () => ({
    page_info: {
      title: "It is a page",
      description:
        "This is a test page with some uncertain content and cat image",
      cat: "https://amplis-online.com/data/command/adding-a-compiled-application-to-path-understanding-the-problem.jpeg",
    },
  }),
};
</script>

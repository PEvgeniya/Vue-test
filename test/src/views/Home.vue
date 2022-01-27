<template>
  <v-container>
    <section>
      <div class="font-weight-medium">
        Hi, stranger. It's been a while. <br />
        <a
          href="https://www.youtube.com/watch?v=lDetXuXJz_0&ab_channel=KirstenLepore"
          target="_blank"
          style="text-decoration: none; color: inherit"
          class="font-italic light-green--text text--{lighten-2}"
          >Click here, if you don't recognize this line.
        </a>
      </div>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <List></List>
      <div class="containerclass">
        <List></List>
        <List></List>
        <List></List>
        <List></List>
        <List></List>
        <List></List>
        <List></List>
        <List></List>
        <List></List>
        <List></List>
      </div>
    </section>
  </v-container>
</template>

<script>
import List from "../components/List.vue";
export default {
  name: "Home",
  components: {
    List,
  },
};
</script>

<style>
.containerclass {
  height: 750px;
  overflow-y: scroll;
}
</style>

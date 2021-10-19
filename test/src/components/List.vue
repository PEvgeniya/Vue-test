<template>
  <v-container>
    <v-card class="mx-auto" max-width="85vw">
      <v-list>
        <v-subheader
          class="text-h5 font-weight-bold light-green--text text--{lighten-2}"
          >Some test pages</v-subheader
        >
        <v-list-item-group v-model="selectedItem" color="light-green lighten-1">
          <v-list-item v-for="item in items" :key="item.id">
            <v-list-item-content>
              <router-link
                style="text-decoration: none; color: inherit"
                to="/listitem/page"
              >
                <v-list-item-title> {{ item.title }} </v-list-item-title>
                <v-list-item-subtitle> {{ item.info }} </v-list-item-subtitle>
              </router-link>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: "List",
  data: () => ({
    items: [
      {
        id: 0,
        title: "First page",
        info: "Just page with any test content",
      },
      {
        id: 1,
        title: "Second page",
        info: "Just another page with the same content",
      },
      {
        id: 2,
        title: "Third page",
        info: "There is nothing interesting here",
      },
    ],
  }),
};
</script>

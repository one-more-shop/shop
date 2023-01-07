<template>
  <div>
    <v-app-bar elevation="4" prominent>
      <v-form @submit.prevent="search">
        <v-container>
          <v-row>
            <v-col cols="8" md="8">
              <v-text-field
                v-model="query"
                label="Search"
                append-icon="mdi-magnify"
              />
            </v-col>
            <v-col cols="4" md="4">
              <v-btn small color="blue" >Search</v-btn>
            </v-col>
          </v-row>
        </v-container>
      </v-form>
    </v-app-bar>
    <nuxt />
  </div>
</template>

<style>
/* Add your styles here */
</style>

<script>
export default {
  data() {
    return {
      query: "",
    };
  },
  methods: {
    search() {
      // Add your search logic here
      console.log(this.query);
    },
  },
};
</script>

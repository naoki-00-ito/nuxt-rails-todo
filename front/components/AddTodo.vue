<template>
  <v-form>
    <v-container>
      <v-form>
        <v-cols col="12" md="4">
          <v-text-field v-model="title" counter="10" label="todo" required>
          </v-text-field>
        </v-cols>

        <v-cols col="12" md="4">
          <v-btn @click="handleSubmit">作成</v-btn>
        </v-cols>
      </v-form>
    </v-container>
  </v-form>
</template>

<script>
export default {
  data() {
    return {
      title: "",
    };
  },

  methods: {
    handleSubmit() {
      this.title = "";
    }
  }
};
</script>

<style>

</style>
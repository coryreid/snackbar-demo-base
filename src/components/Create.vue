<template>
<v-flex>
  <v-btn @click="openSnackbar">Create</v-btn>
  <v-btn to="/">Return Home</v-btn>
</v-flex>
</template>

<script>
import { mapMutations } from "vuex";
export default {
  data() {
    return {}
  },
  methods: {
    ...mapMutations(["showSnackbar", "closeSnackbar"]),
    openSnackbar() {
      this.showSnackbar({ text: "You created something!" })
    }
  }
}
</script>

<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      
    </v-app-bar>

    <v-main>
      <v-app class="d-flex flex-column align-center">
        <v-sheet width="100">
          <v-row class="ma-4 pa-0">
            Counter: 
            <v-text-field readonly :value="counter" outlined></v-text-field>
          </v-row>
          <v-btn color="primary" @click="incrementCounter">Increment</v-btn>
        </v-sheet>
        
        <!-- TODO: table here -->

      </v-app>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App',

  components: {
  },

  data: () => ({
    
  }),
  computed: {
    counter() {
      return this.$store.state.counter
    }
  },
  methods: {
    incrementCounter() {
      this.$store.commit('setCounter', this.counter + 1)
    }
  }
};
</script>

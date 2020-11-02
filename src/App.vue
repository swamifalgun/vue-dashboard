<template>
  <v-app>
    <v-main>
      <v-container class="dashboard">
          <div>
            <div class="transport">
              <BusChart />
            </div>
            <div class="electricity">
              <h1>Electricity</h1>
            </div>
          </div>
          <div class="weather">
            <h1>Weather</h1>
          </div>
      </v-container>
      
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import BusChart from './components/BusChart';

export default {
  name: 'App',

  components: {
    HelloWorld,
    BusChart
  },

  data: () => ({
    //
  }),
};
</script>

<style scoped lang="scss">
  .dasboard {
    display: flex;
    flex-direction: row;
    border: 1px solid black;
  }

  .transport {
    width: 500px;
    height: 200px;
    border: 1px solid red;
  }

  .electricity {
    border: 1px solid green;
    width: 500px;
    height: 200px;
  }

  .weather {
    align-items: baseline;
    width: 200px;
    height: 200px;
    border: 1px solid blue;
  }
</style>

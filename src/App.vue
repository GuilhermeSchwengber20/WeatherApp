<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input
          type="text"
          class="search-bar"
          placeholder="Search..."
          v-model="query">
      </div>
      <div class="weatherApp">
        <div class="locationBox">
          <div class="location"></div>
          <div class="date"></div>
        </div>

        <div class="weather-box">
          <div class="temp"></div>
          <div class="weather"></div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return{
      api_key: 'f6a2c317f97367bfe8fa3e5fc517e80d',
      url_base: 'https://api.openweathermap.org/data/2.5/',
      query: '',
      weather: {}
    }
  },
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


</style>

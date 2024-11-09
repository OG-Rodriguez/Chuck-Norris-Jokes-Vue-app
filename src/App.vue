<template>
  <div id="app" class="container">
    <h1>Chuck Norris Jokes</h1>
    <div class="row">
      <chuck-card
        v-for="(joke, index) in chuck"
        :key="index"
        :icon_url="joke.icon_url"
        :value="joke.value"
        class="col-md-4 col-sm-12 mb-4"
      />
    </div>
  </div>
</template>

<script>
import ChuckCard from './components/ChuckCard.vue';

export default {
  name: 'App',
  components: {
    ChuckCard
  },
  data() {
    return {
      chuck: [
        { icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png", value: "Chuck Norris can skydive into outer space." },
        { icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png", value: "The chief export of Chuck Norris is pain." },
        { icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png", value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png", value: "Time waits for no man. Unless that man is Chuck Norris." },
        { icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png", value: "If you spell Chuck Norris in Scrabble, you win. Forever." }
      ]
    };
  }
};
</script>

<style scoped>
/* Styling for the app */
#app {
  font-family: 'Helvetica Neue', sans-serif;
  text-align: center;
  margin-top: 20px;
}

h1 {
  color: #4A90E2; /* Blue color */
  font-size: 2.5em; /* Increased font size */
  font-family: 'Georgia', serif; /* Different font family */
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  padding: 15px;
  margin: 15px auto;
  max-width: 600px;
  background-color: #EFEFEF; /* Lighter grey background */
  border: 1px solid #B0BEC5; /* Different border color */
  border-radius: 12px; /* More rounded corners */
  color: #333; /* Darker text color */
  font-size: 1.2em; /* Larger font size */
  font-family: 'Verdana', sans-serif; /* Different font family */
}
</style>



<template>
  <div id="app">
    <h1>Chuck Norris Jokes</h1>
    <ul>
      <!-- Loop through the jokes array and display each joke in a list item -->
      <li v-for="(joke, index) in chuck" :key="index">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      chuck: [
        { value: "Chuck Norris can skydive into outer space." },
        { value: "The chief export of Chuck Norris is pain." },
        { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { value: "Time waits for no man. Unless that man is Chuck Norris." },
        { value: "If you spell Chuck Norris in Scrabble, you win. Forever." }
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



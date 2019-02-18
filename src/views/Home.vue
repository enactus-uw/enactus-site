<template>
  <div class="home">
    <div class="introduction">
      <img alt="Team Picture" src="../assets/team.png" id="team">
      <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
      <div class="textnbutton">
        <h1 id="intro">
          ENACTUS IS A COMMUNTIY OF ENTREPRENURIAL LEADERS WHO SEE BUSINESS AS A
          WAY TO ADDRESS SOCIAL ISSUES
        </h1>
        <button type="button" id="learn-more">LEARN MORE</button>
      </div>
    </div>
    <div class="intro-projects">
      <h1 id="projects">PROJECTS</h1>
      <hr>
    </div>
    <div class="joining-team">
      <div class="textnbutton" id="join-team-textnbutton">
        <h1 id="interested">INTERESTED IN JOINING THE TEAM?</h1>
        <router-link to="/recruitment" id="avail-positions-button">AVAILABLE POSITIONS</router-link>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "home",
  // components: {
  //   HelloWorld
  // }
};
</script>

<style lang="scss">
#intro {
  text-align: left;
  font-weight: bold;
  font-size: 2.8vw;
  margin: 0;
  padding-bottom: 1vh;
  word-wrap: normal;
}

#team {
  width: 45%;
  padding-right: 7vw;
}

.introduction {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 5vw;
  background-color: #1a1a1a;
  color: white;
  height: 69vh;
}

.textnbutton {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  // margin: 0;
  // height: 80%;
  width: 41%;
}

#learn-more {
  background-color: #fec222;
  padding: 1.5vh 0vw;
  margin-top: 2vh;
  width: 50%;
  border: none;
  font-size: 1.5vw;
  border-radius: 12px;
  font-weight: bold;

  cursor: pointer;
}

/////////////////////////////
// PROJECT SAMPLE
/////////////////////////////

.intro-projects {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  padding: 10vh;
  background-color: white;
  height: 80vh;
}

#projects {
  margin: 0;
  font-size: 2.8vw;
}

/////////////////////////////
// JOINING THE TEAM
/////////////////////////////

.joining-team {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 10vh;
  background-color: #ffb801;
  height: 80vh;
  font-size: 2vw;
}

#interested {
  color: white;
}

#avail-positions-button {
  background-color: #1a1a1a;
  padding: 1.5vw 1.2vw;
  margin-top: 2vh;
  width: 55%;
  border: none;
  font-size: 2.3vw;
  font-weight: bold;
  color: #fec222;
  cursor: pointer;
  text-decoration: none;
}

#join-team-textnbutton {
  align-items: center;
  width: 60%;
}
</style>

<template>
  <div id="heroes">
    <ul>
      <li v-for="hero in heroes" @click="hero.show = !hero.show">
        <h2>{{ hero.superhero }}</h2>
        <h3 v-show="hero.show">{{ hero.characters }}</h3>
        <p>
          <img v-show="hero.show" v-bind:src="hero.image" alt="" height="150px" width="300px">
        </p>
      </li>
    </ul>
  </div>
</template>

<script>

export default {
  data () {
    return {
      heroes:[
              {
                  superhero:"Batman",
                  publisher:"DC Comics",
                  characters:"Bruce Wayne",
                  image: '../src/assets/batman.jpg',
                  show: false
              },
              {
                  superhero:"Superman",
                  publisher:"DC Comics",
                  characters:"Kal-El",
                  image: '../src/assets/superman.jpg',
                  show: false
              },
              {
                  superhero:"Flash",
                  publisher:"DC Comics",
                  characters:"Jay Garrick, Barry Allen, Wally West, Bart Allen",
                  image: '../src/assets/flash.jpg',
                  show: false
              },
              {
                  superhero:"Green Lantern",
                  publisher:"DC Comics",
                  characters:"Alan Scott, Hal Jordan, Guy Gardner, John Stewart, Kyle Raynor, Jade, Sinestro, Simon Baz",
                  image: '../src/assets/green.jpg',
                  show: false
              },
              {
                  superhero:"Green Arrow",
                  publisher:"DC Comics",
                  characters:"Oliver Queen",
                  image: '../src/assets/greenArrow.jpg',
                  show: false
              },
              {
                  superhero:"Wonder Woman",
                  publisher:"DC Comics",
                  characters:"Princess Diana",
                  image: '../src/assets/wonderwoman.jpg',
                  show: false
              },
              {
                  superhero:"Martian Manhunter",
                  publisher:"DC Comics",
                  characters:"Martian Manhunter",
                  image: '../src/assets/manhunter.jpg',
                  show: false
              },
              {
                  superhero:"Robin/Nightwing",
                  publisher:"DC Comics",
                  characters:"Dick Grayson",
                  image: '../src/assets/robin.jpg',
                  show: false
              },
              {
                  superhero:"Blue Beetle",
                  publisher:"DC Comics",
                  characters:"Dan Garret, Ted Kord, Jaime Reyes",
                  image: '../src/assets/bluebeetle.jpg',
                  show: false
              },
              {
                  superhero:"Black Canary",
                  publisher:"DC Comics",
                  characters:"Dinah Drake, Dinah Lance",
                  image: '../src/assets/canary.jpg',
                  show: false
              },
              {
                  superhero:"Spider Man",
                  publisher:"Marvel Comics",
                  characters:"Peter Parker",
                  image: '../src/assets/spiderman.jpg',
                  show: false
              },
              {
                  superhero:"Captain America",
                  publisher:"Marvel Comics",
                  characters:"Steve Rogers",
                  image: '../src/assets/captianamerica.jpg',
                  show: false
              },
              {
                  superhero:"Iron Man",
                  publisher:"Marvel Comics",
                  characters:"Tony Stark",
                  image: '../src/assets/ironman.jpg',
                  show: false
              },
              {
                  superhero:"Thor",
                  publisher:"Marvel Comics",
                  characters:"Thor Odinson",
                  image: '../src/assets/thor.jpg',
                  show: false
              },
              {
                  superhero:"Hulk",
                  publisher:"Marvel Comics",
                  characters:"Bruce Banner",
                  image: '../src/assets/hulk.png',
                  show: false
              },
              {
                  superhero:"Wolverine",
                  publisher:"Marvel Comics",
                  characters:"James Howlett",
                  image: '../src/assets/wolverine.jpg',
                  show: false
              },
              {
                  superhero:"Daredevil",
                  publisher:"Marvel Comics",
                  characters:"Matthew Michael Murdock",
                  image: '../src/assets/daredevil.jpg',
                  show: false
              },
              {
                  superhero:"Hawkeye",
                  publisher:"Marvel Comics",
                  characters:"Clinton Francis Barton",
                  image: '../src/assets/hawkeye.jpg',
                  show: false
              },
              {
                  superhero:"Cyclops",
                  publisher:"Marvel Comics",
                  characters:"Scott Summers",
                  image: '../src/assets/cyclops.jpg',
                  show: false
              },
              {
                  superhero:"Silver Surfer",
                  publisher:"Marvel Comics",
                  characters:"Norrin Radd",
                  image: '../src/assets/silversurface.png',
                  show: false
              }
          ]
    }
  }
}
</script>

<style scoped>
#heroes{
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}
ul{
  display: flex;
  flex-wrap: wrap;
  list-style-type:none;
  padding: 0;
}
li{
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  margin: 10px;
}
</style>

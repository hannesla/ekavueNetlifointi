<template>
  <div class="hello">
      {{msg}} <br />
      {{yksinkertainen}}<br />
      {{palautettavaaDataa[0].kivaNumero}}
      <div v-bind:key="tavara.kivaNumero" v-for="tavara in palautettavaaDataa">
          {{tavara}}
      </div>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/JcopYjDomao" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    yksinkertainen: String
  },
  methods: {
    esimerkkiMetodi() {

    }
  },
  data() {
    return {
      palautettavaaDataa: 
        [
          {
            kivaNumero: 12345678
          },
          {
            kivaNumero: 123456780
          }
        ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

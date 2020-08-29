<template>
  <div class="hello">
      {{msg}} <br />
      {{yksinkertainen}}<br />
      {{palautettavaaDataa[0].kivaNumero}}
      <div v-bind:key="tavara.kivaNumero" v-for="tavara in palautettavaaDataa">
          {{tavara}}
      </div>
      <iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/748891168&color=%2300ff55&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe><div style="font-size: 10px; color: #cccccc;line-break: anywhere;word-break: normal;overflow: hidden;white-space: nowrap;text-overflow: ellipsis; font-family: Interstate,Lucida Grande,Lucida Sans Unicode,Lucida Sans,Garuda,Verdana,Tahoma,sans-serif;font-weight: 100;"><a href="https://soundcloud.com/metaru87" title="metaru" target="_blank" style="color: #cccccc; text-decoration: none;">metaru</a> · <a href="https://soundcloud.com/metaru87/my-first-song-heavenly-edition" title="My First Song Heavenly Edition" target="_blank" style="color: #cccccc; text-decoration: none;">My First Song Heavenly Edition</a></div>
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

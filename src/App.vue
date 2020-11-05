<template>
  <div id="app">
    <Navbar />
    <img class="columns is-vcentered" src="./assets/mountain.jpg">
    <footer class="footer">
      <div class="content has-text-centered">
        <p>
          <strong>ŠTO KAŽU NAŠI IZLETNICI..</strong>
          <br/>
          <br/>
          Odlično iskustvo s raspoloženom i nasmijanom ekipom!
          <br/>
          <strong>Ana Čuljak, Zagreb</strong>          
          <br/>
          Prošao sam nekoliko izleta i avantura s Mountain match i uvijek nam je bilo lijepo i jedva čekam sljedeći put!
          <br/>
          <strong>Marko Radoš, Sisak</strong>
        </p>
      </div>
    </footer>    
  </div>
</template>

<script>
import Navbar from './components/Navbar';

export default {
  name: 'App',
  components: {
    Navbar
  }
}
</script>




<style>
*{margin:0;padding:0;}
img{width:70%;margin:0 auto;}


</style>

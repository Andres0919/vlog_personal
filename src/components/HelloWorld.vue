<template>
  <div>
    <header>
      <label>Andrés Posada</label>
      <p @click="toggleMenu" >Menú</p>
    </header>
    <transition name="fade">
    <div v-if="showMenu" id="menu"> 
      <p @click="toggleMenu" > X </p>
      <ul>
        <li>Inicio</li>
        <li>Perfil</li>
        <li>Ingresar</li>
      </ul>
    </div>
    </transition> 
    <div id="introduce">
      <h2>ANDRÉS POSADA</h2>
      <h3>DESAROLLADOR WEB JR</h3>
      <img src="https://uploads-ssl.webflow.com/593008e46c534e61e392e0f2/59326fbebaf9b1348967fa14_sep-white.svg" />
    </div>
    <div id="social-media">
      <span>Facebook</span>
      <span>Twitter</span>
      <span>Github</span>
      <span>Linkedin</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },  
  data(){
    return({
      showMenu: false
    });
  },
  methods:{
    toggleMenu: function() {
      this.showMenu = !this.showMenu;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 25px
}

header label, header p{
  font-size: 2em;
  font-weight: bold;
  font-family: 'Clicker Script', cursive;
  cursor: pointer;
  padding: 10px;
  border-radius: 5px;
}

header p:hover{
  background-color: #fff;
  color: #000;
}

h2 {
  font-size: 500%;
}

h3{
  font-size: 100%;
  margin-bottom: 60px;
}

#menu{
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 85%; 
  background-color: #fff;
}

#menu p{
  position: relative;
  width: 5%;
  padding: 5px;
  margin: 5px;
  font-size: 1em;
  text-align: center; 
  border-radius:50%;
  cursor: pointer;
}

#menu p:hover{
  background-color: #555;
  color: #fff;
}

#menu li{
  text-align: left;
}

#menu li, #menu p{
  list-style: none;
  color: #000;
}

#introduce{
  position: absolute;
  top: 35%;
  width: 100%;
  text-align: center;
  font-family: 'Raleway', sans-serif;
}

.fade-enter-active, .fade-leave-active {
  transition: ease-out .5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
#social-media{
  position: absolute;
  top: 90%;
  right: 0;
  bottom: 0;
}

#social-media span{
  margin: 0 15px;
}

</style>

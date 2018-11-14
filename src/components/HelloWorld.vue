<template>
  <div>
    <header>
      <p>Andrés Posada</p>
      <p>Menú</p>
    </header>
    <div id="introduce">
      <h2>ANDRÉS POSADA</h2>
      <h3>DESAROLLADOR WEB JR</h3>
      <img src="https://uploads-ssl.webflow.com/593008e46c534e61e392e0f2/59326fbebaf9b1348967fa14_sep-white.svg" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
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

header p{
  font-size: 2em;
  font-weight: bold;
  font-family: 'Clicker Script', cursive;
}

h2 {
  font-size: 500%;
}

h3{
  font-size: 100%;
  margin-bottom: 60px;
}

#introduce{
  position: absolute;
  top: 35%;
  width: 100%;
  text-align: center;
  font-family: 'Raleway', sans-serif;
}

</style>

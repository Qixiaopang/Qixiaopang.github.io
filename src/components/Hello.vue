<template>
  <div class="hello">
  	<div class="center">
  		 <h1>{{ msg }}</h1>
  		 
  	</div>
    
    
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'my resume'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
.hello{
	width: 100%;
	height: 340px;
	background: #fff;
}
.center{
	width: 1075px;
	height: 280px;
	padding: 60px 0 0 0;
	background: pink;
	margin: 0 auto;
}
</style>

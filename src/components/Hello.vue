<template>
	<div class="hello">
<div class="container">

<div class="navbar">MENU</div>
<div class="timeline">timeline</div>
<div class="main">


<div class='component'>
<section class='top'>
</section>
<div class="photo">
<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/adellecharles/128.jpg"></img>
</div>
<h3 class="name">Jenny</h3>
<h4 class="addr">Jen@toiyp.me</h4>
<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 width="64px" height="64px" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve">
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M54,64c0,0-6-5-6-12s0-40,0-40s0-11-8-11s-8,11-8,11
	v40"/>
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M16,52V12c0,0,0.083-11,8-11s8,11,8,11"/>
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M16,12c0,0,0-10-8-10"/>
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M48,24c0,0,0-14,6-14s6,14,6,14s-1,34-27,34"/>
</svg>
<section class='bottom bottom--female'>
</section>


</div>


<div class='component'>
<section class='top'>
</section>
<div class="photo">
<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/peterme/128.jpg">
</div>
<h3 class="name">Rupert</h3>
<h4 class="addr">RuMeister@toiyp.me</h4>
<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 width="64px" height="64px" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve">
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M41.667,38.002
	c3.913-2.939,6.444-7.619,6.444-12.891C48.111,16.213,40.897,9,32,9s-16.111,7.213-16.111,16.111c0,5.27,2.53,9.948,6.442,12.889"/>
<line fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" x1="0" y1="38" x2="23" y2="38"/>
<line fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" x1="41" y1="38" x2="64" y2="38"/>
<line fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" x1="0" y1="55" x2="64" y2="55"/>
</svg>
<section class='bottom bottom--male'>
</section>


</div>



<div class='component'></div>
<div class='component'></div>
<div class='component'></div>
<div class='component'></div>
<div class='component'></div>
<div class='component'></div>

</div>
</div>
	</div>
</template>

<script>
	export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


.container {
	display: grid;
  height: 100vh;
  width: 100vw;
	grid-template-columns: minmax(min-content, 200px) minmax(min-content, 150px) 1fr;
  margin: 0px 1px;
}

.navbar {
	
  background-color: orange;
  color: white;
  font-weight: 600;
  grid-row: 2 / 3;
  margin-top: 15px;
  padding: 30px 10px;
  box-shadow: 0px 4px 20px rgba(0,0,0, .2);
}


.timeline {
  grid-column: 2;
  grid-row: 3 / -1;
  max-width: 150px;
  margin-top: 15px;
  margin-left: 20px;
  padding: 30px 10px;
  box-shadow: 0px 4px 20px rgba(0,0,0, .2);
}

.main {
  
  grid-column: 3 / -1;
  grid-row: 2;
  display: grid;
  grid-template-columns:repeat(auto-fit, minmax(350px, 1fr));
  grid-template-rows: repeat(10,1fr);
  grid-gap: 12px;
  margin: 10px 10px;
  margin-right: 50px;
}

.component{
  background-color: #fff;
  height: 150px;
  width: 100%;
  border-radius: 5px;
  box-shadow: 0px 4px 20px rgba(0,0,0, .2);
  transition: all .2s;
  border: 1px solid peachpuff;

  margin: 5px;
  text-align: left;
  display: grid;
  grid-template-columns: repeat(5, min-max(10px, 20%));
  grid-template-rows: 20% 20% [bottom-start] 20% 20% 20% [bottom-end];
  grid-gap: 5px;
  
  overflow: hidden;
}

.component:hover {
  transform: scale(1.05);
}

.component:active {
  transform: rotateY(90deg);
}

.bottom {
  grid-row: 4;
  grid-column-start: 1;
  grid-column-end: 5;
  height: 80px;
  width: 130%;
  display: block;
  background-color:blueviolet;
  
  padding: 10px;
  transform: rotate(-5deg) translateY(-15px);
  opacity: .5;
}

 .bottom--male {
    background-color: lightskyblue;
  }

.top {
  grid-row: 1 / 6;
  grid-column-start: 1;
  grid-column-end: 5;
  background-color: white;
}

.addr {
  font-size: 15px;
  grid-row: 2;
  grid-column: 3; 
  color: #444;
  font-weight: 300;

}

.name {
  grid-row: 2;
  grid-column: 3; 
  color: #444;
   transform: translateY(-20px);
  
}

.photo {
  grid-column: 1 / span 2;
  grid-row-start: 1;
  width: 150px;
  height: 300px;
  background-color: orange;
  transform: rotate(10deg) translateY(15px) translateX(-10px);
  z-index: 99;
  border-radius: 5px;
  margin-right: 10px;
}

.avatar {
  width: 100px;
  height: 100px;
  border: solid 1px white;
  border-radius: 50%;
  margin: 20px auto;
  transform: translateX(22px) rotate(-10deg);
  transition: all .6s;
}


.icons {
  color: white;
  grid-column: 3 /span 3;
  grid-row: 4 /span 2;
  z-index: 100;
  transform: translateY(-15px);

}

svg {
  width: 15px;
  gid-column: 1 / 2;
  grid-row: 3;
}



@media (max-width: 600px) {
  .navbar {
    grid-row: 1;
    grid-column: 1 / -1;
    padding: 10px;
  }

  .timeline {
     grid-row: 2;
   grid-column: 1 / -1;
   height: 15px;
   max-width: 85vw;
   z-index: -0;
  }

.main {
grid-column: 1 / -1;
grid-row: 3;
}


  


}
</style>
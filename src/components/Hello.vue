<template>
	<div class="hello">
<div class="container">

<div class="navbar">
<div class="navbar__header">
<img class="avatar avatar-big" src="https://images.unsplash.com/photo-1476900966873-ab290e38e3f7?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&cs=tinysrgb&w=200&fit=max&s=fe0976a79ece0ee8effca4cab4527ae2">
<h4 class="handle">Barabus</h4>
</div>
</div>
<div class="timeline">

<div class="timeline-header">
<svg class="icon_big" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 width="64px" height="64px" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve">
<path fill="none" stroke="#ffffff" stroke-width="3" stroke-linejoin="bevel" stroke-miterlimit="10" d="M63.051,56
	c0-13.416-4.804-25.711-12.786-35.256"/>
<path fill="none" stroke="#ffffff" stroke-width="3" stroke-linejoin="bevel" stroke-miterlimit="10" d="M50.265,20.744
	C40.177,8.677,25.01,1,8.051,1"/>
<path fill="none" stroke="#ffffff" stroke-width="3" stroke-linejoin="bevel" stroke-miterlimit="10" d="M51.769,56
	c0-24.145-19.574-43.718-43.718-43.718"/>
<path fill="none" stroke="#ffffff" stroke-width="3" stroke-linejoin="bevel" stroke-miterlimit="10" d="M40.486,56
	c0-17.913-14.523-32.436-32.436-32.436"/>
<path fill="none" stroke="#ffffff" stroke-width="3" stroke-linejoin="bevel" stroke-miterlimit="10" d="M29.205,56
	c0-11.684-9.472-21.154-21.154-21.154"/>
<circle fill="none" stroke="#ffffff" stroke-width="4" stroke-linejoin="bevel" stroke-miterlimit="10" cx="8.051" cy="56" r="7.051"/>
</svg>
</div>
<div class="event">
<h4 class="event-day">
Today</h4>
</div>
<div class="event">
<h4 class="event-day">
Yesturday</h4>
</div>
<div class="event">
<h4 class="event-day">
Last Week</h4>
</div>
</div>
<div class="main">
<div class='component'>
<section class='top'>
</section>
<div class="photo">
<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/adellecharles/128.jpg"></img>
</div>
<h3 class="name">Jenny</h3>
<h4 class="addr">Jen@toiyp.me</h4>

<section class='bottom bottom--female'>
</section>
<div class="side-tab">
<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 width="64px" height="64px" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve">
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M54,64c0,0-6-5-6-12s0-40,0-40s0-11-8-11s-8,11-8,11
	v40"/>
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M16,52V12c0,0,0.083-11,8-11s8,11,8,11"/>
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M16,12c0,0,0-10-8-10"/>
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M48,24c0,0,0-14,6-14s6,14,6,14s-1,34-27,34"/>
</svg>
</div>


</div>


<div class='component'>
<section class='top'>
</section>
<div class="photo">
<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/peterme/128.jpg">
</div>
<h3 class="name">Rupert</h3>
<h4 class="addr">RuMeister@toiyp.me</h4>
<div class="side-tab">
<svg version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
	 width="64px" height="64px" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve">
<path fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" d="M41.667,38.002
	c3.913-2.939,6.444-7.619,6.444-12.891C48.111,16.213,40.897,9,32,9s-16.111,7.213-16.111,16.111c0,5.27,2.53,9.948,6.442,12.889"/>
<line fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" x1="0" y1="38" x2="23" y2="38"/>
<line fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" x1="41" y1="38" x2="64" y2="38"/>
<line fill="none" stroke="#000000" stroke-width="2" stroke-miterlimit="10" x1="0" y1="55" x2="64" y2="55"/>
</svg>
</div>
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

import '../assets/icons.svg';
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

.hello {
  background-color: antiquewhite;
  height: 100vh;
  z-index: -10;
}

.container {
	display: grid;
  height: 100vh;
  width: 100vw;
	grid-template-columns: minmax(min-content, 200px) minmax(min-content, 200px) 1fr;
  margin: 0px 10px;
}

.navbar {
	border-radius: 5px;
  background-color: orange;
  color: white;
  font-weight: 600;
  grid-row: 2 / 3;
  margin-top: 15px;
  box-shadow: 0px 4px 20px rgba(0,0,0, .2);

  display: grid;
  grid-template-rows: repeat(5, minmax(min-content,1fr));
}

.navbar__header{
  height: 190px;
  background-color: white;
  clip-path: polygon(0 0, 0% 100%, 100% 85%, 100% 0%);
  border-bottom: solid 1px white;
}


.timeline {
  grid-column: 2;
  grid-row: 3 / -1;
  max-width: 200px;
  margin-top: 15px;
  margin-left: 20px;
 border-radius: 5px;
  box-shadow: 0px 4px 20px rgba(0,0,0, .2);
  background-color: white;
  display: grid;
  grid-template-rows: repeat(11, minmax(min-content, 1fr));
  align-items:top;
  overflow: hidden;
  
 
}

.timeline-header {
  background-color: orange;
  height: 30px;
  grid-row: 1;
  z-index: 1;
  padding: 30px 5px;
   clip-path: polygon(0 0, 0% 100%, 100% 85%, 100% 0%);
  //transform: rotate(-5deg) translateX(-10px) translateY(-10px);
}

.event {
  border-radius: 10;
  padding: 10px 0;
  margin: 5px;
  margin-bottom: 5px;

  display: grid;
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

.event-day {
  color: #ccc;
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
  grid-template-columns:  170px minmax(min-content, 1fr) minmax(min-content, 1fr);
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

.side-tab {
 background-color: rgba(250,115,50, .5);
 border-left: 1px solid white;
 grid-row: 1 / -1;
 width: 50px;
 z-index: 200;
 float: right;
 text-align: center;
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
  font-size: 12px;
  line-height: 2.5;
  grid-row: 2;
  grid-column: 2; 
  color: #444;
  font-weight: 300;

}

.name {
  grid-row: 2;
  grid-column: 2; 
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

.avatar-big {
  width: 100px;
  height: 100px;
  border: solid 2px orange;
  transform: rotate(3deg);

}

.handle {
  transform: translateY(-27px);
  color: black;
}

.icons {
  color: white;
  grid-column: 3 /span 3;
  grid-row: 4 /span 2;
  z-index: 100;
  transform: translateY(-15px);

}

svg {
  width: 20px;
}

.icon_big {
  width: 40px;
  height: 40px;
  opacity: .4;
}


@media (max-width: 600px) {
  .navbar {
    grid-row: 1;
    grid-column: 1 / -1;
    padding: 0px 0px;
    height: 70px;
    overflow: visible;
  }

  .avatar-big {
    width: 70px;
    height: 70px;
    grid-row: 1;
    visibility: hidden;
  }

.navbar__header {
  background-color: orange;
 height: 0%;
 visibility: none;
 
 padding: 0px 0px;
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
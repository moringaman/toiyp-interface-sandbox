<template>

<div class='component'>
<section class='top'>
</section>
<div class="photo">
<div class="">
<slot name="avatar">
</slot>
</div>
</div>
<div class="name">
<slot name="name">
</slot>
</div>
<div class="addr">
<slot name="addr">
</slot>
</div>

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

<div v-if="gender!=='female'" class="bottom bottom--male" >
</div>
<div v-else class="bottom">></div>
</div>

</div>

</template>

<script>
export default {
 props: [ 'gender' ]
}
</script>

<style>
.component{
  background-color: #fff;
  height: 150px;
  width: 100%;
  border-radius: 5px;
  box-shadow: 0px 4px 20px rgba(0,0,0, .2);
  transition: all .2s;
  // border: 1px solid peachpuff;

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

svg {
  width: 20px;
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

</style>

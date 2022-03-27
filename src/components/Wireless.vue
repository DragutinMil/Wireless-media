<template>
  <div class="home">
    <div id="header">
      <img src="../assets/WMv1_04.jpg" id="logo"  alt="">   
      <div id="header_menu">
         <p class="hm2-1"> HOME </p> &nbsp;&nbsp;<p> /</p>&nbsp;&nbsp;
         <p class="hm2-2"> ABOUT US </p> &nbsp; &nbsp;<p> /</p>&nbsp;&nbsp;
         <p class="hm2-3"> OUR WORK </p> &nbsp;&nbsp;<p>/</p>&nbsp;&nbsp;
         <p class="hm2-4"> CONTACT </p> &nbsp;&nbsp;
      </div>
      <div id="header_menu2">
         <i  class="fa-solid fa-house padd hm2-1"></i>
         <i  class="fa-solid fa-circle-question padd hm2-2"></i>
         <i  class="fa-solid fa-graduation-cap padd hm2-3"></i>
         <i  class="fa-solid fa-envelope padd hm2-4"></i>
      </div>
        
      <div class="centered" >
         <i @click="expanded_manu=!expanded_manu" id="header_menu3" class="fa-solid fa-bars"></i>
      </div>
      <i @click="search_true=!search_true" id="search-button" class="fa-solid fa-magnifying-glass"></i>
      
     
    </div>
    <input v-if="search_true"  type="text" name="" id="input_field" >
    <div v-if="expanded_manu" class="exp_part" >
       <div class="exp_parts" style="background-color:#9fc360">HOME</div>
       <div class="exp_parts" style="background-color:#a3d4dc">ABOUT US</div>
       <div class="exp_parts" style="background-color:#80b4c8">OUR WORK</div>
       <div class="exp_parts" style="background-color:#2d82ac">CONTACT</div>
    </div>
	  <img id="hr" src="../assets/WMv13333_06.jpg"  alt=""> 
	  <img src="../assets/WMv13333_08.jpg" id="after_header"  alt=""> 
    <div id="after_header3">
      <img src="../assets/WMv99999_07.jpg"   alt=""> 
      <img src="../assets/WMv99999_09.jpg"   alt=""> 
    </div>
  	<div>
		  <h1>WHO WE ARE</h1>
	  </div>
    <div class="grig_part">
      <div class="gray_part">
        <i  class="fa-solid fa-graduation-cap"></i>
      </div>
      <div>
        <h3>Lorem ipsum</h3>
        <p class="text_middle">
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
        Distinctio mollitia rerum laudantium culpa.
        </p>
        <div class="link-button">
          <a href="" class="show_button">SHOW MORE</a>
        </div>
      </div>
    </div>
    <div class="grig_part">
      <div class="gray_part">
          <i class="fa-solid fa-thumbs-up"></i>
      </div>
    <div>
      <h3>Lorem ipsum </h3>
      <p class="text_middle">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. 
      </p>
      <div class="link-button">
        <a href="" class="show_button">SHOW MORE</a>
      </div>
    </div> 
    </div>
    <div>
      <h1>WHAT WE DO</h1>
    </div>
    <div>
      <div class="grig_part">
        <div class="gray_part">
          <i class="fa-solid fa-calculator"></i>
        </div>
        <div class="gray_part">
          <i class="fa-solid fa-cloud"></i>
        </div>
      </div>
    </div>
    <div>
      <div class="grig_part">
        <div class="gray_part">
          <i class="fa-solid fa-clock"></i>
        </div>
        <div class="gray_part">
          <i class="fa-solid fa-heart"></i>
        </div>
      </div>
    </div>
    <footer>
      <div style="display:flex">
        <div class="white_circle">
          <i class="fa-brands fa-facebook-f"></i>
        </div>
        <div class="white_circle">
          <i class="fa-brands fa-twitter"></i>
        </div>
        <div class="white_circle">
          <i class="fa-solid fa-envelope"></i>
        </div>
      </div>
      <div id="footer_menu">
          <p> HOME </p> &nbsp;&nbsp;&nbsp;&nbsp;
          <p> ABOUT US </p> &nbsp; &nbsp;&nbsp;&nbsp;
          <p> OUR WORK </p> &nbsp;&nbsp;&nbsp;&nbsp;
          <p> CONTACT </p> &nbsp;&nbsp;
        </div>
        <div class="white_circle">
          <i class="fa-solid fa-arrow-up"></i>
        </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'Wireless',
  props: {
  },
  data() {
    return {
      search_true: false,
      expanded_manu:false
    };
  },
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

body{
  margin:0;
  padding:0;
}
h1{
  color:#9e9e9d;
  text-align: left;
  padding-left:19%;
  font-weight: 500;
  margin-top:50px;
}
h3{
  font-size: 14px;
  color:#9e9e9d;
  text-align: left;
}
p{
  font-size: 12px;
  text-align: left;
}

footer{
  background-color: #dbdbdb;
  display:flex;
  justify-content:space-between;
  align-items: center;
  padding:5px 20px 2px 20px;
  margin-top:30px;
}
.gray_part{
  background-color:#f1f1f1;
  height: 120px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 28px;
  color:#9e9e9d;
}
.centered{
  display: flex;
  justify-content: center;
  align-items: center;
}
.gray_part:hover{
  color:#9fc360
}
.text_middle{
  color:#9e9e9d;
}
.home{
	margin:auto;
	width:765px;
}
.link-button{
  background-color: #f1f1f1;
  width:85px;
  font-size: 12px;
  height: 18px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 4px;
  position:relative;
  left:70%
}
.link-button:hover{
  background-color:#9fc360 ;
}

.show_button:hover{
   color:white;
}

.padd{
  font-size: 18px;
  padding-left:15px;
}
.white_circle{
  width: 30px;
  background-color: #FFFFFF;
  height: 30px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left:10px;
}
.white_circle:hover{
  color:#9fc360;
}
.white_circle:visited{
  color:#9fc360;
}
#search-button{
  color:#c6c6c7;
  display: flex;
  justify-content: center;
  align-items: center;
  padding-bottom: 15px;
}
#search-button:hover{
  color:#9fc360;
}

.grig_part{
  padding:20px 10%;
  display:grid;
  grid-template-columns: 45% 45%;
  gap:10%;
}
.show_button{
   text-decoration: none;
}

#hr{
  width:765px;
}
#header{
  display:flex;
  justify-content:space-between;
  width:765px;
  background-color:#fbfbfa;
  margin:auto;
  padding:5px 15px;
  box-sizing: border-box;
}
#header_menu{
  display: flex;
  justify-content: center;
  align-items: center;
  padding-bottom:10px;
  color:#c6c6c7;
  font-size: 20px;
  cursor: pointer;
  font-weight: 600;
}

#header_menu2{
  display:none;
  color:#c6c6c7;
}
#header_menu3{
  display:none;
  
}
#header_menu3:hover{
  color:#9fc360;
}
#footer_menu{
  display: flex;
  justify-content: center;
  align-items: center;
  padding-bottom:5px;
  padding-top:5px;
  color:#858585;
  font-size: 18px;
  cursor: pointer;
}
#after_header3{
  display:none;
}
#search_icon{
  height: 30px;
  padding-top:15px;
  padding-right:10px;
}
#input_field{
  display:none;
}
.hm2-1:hover{
  color:#9fc360;
}
.hm2-2:hover{
  color:#a3d4dc;
}
.hm2-3:hover{
  color:#80b4c8;
}
.hm2-4:hover{
  color:#2d82ac;
}
footer>img{
  height: 25px;

}


@media only screen and (max-width: 768px) {
#footer_menu{
  display: none;
}
.home{
	width:480px;
}
#after_header{
  width: 480px;
}
#header{
   width: 480px; 
}
#hr{
  width:480px;
}
#header_menu{
  display: none;
}
#header_menu2{
  display:none;
}
#header_menu2{
  display:flex;
  height: 20px;
  justify-content: center;
  align-items: center;
  padding-top:18px;
}
#header_menu2>img{
  height: 28px;
}
#input_field{
  display:block;
  margin:auto;
  width:85%;
  border:1px solid #c6c6c7;
  border-radius: 3px;
}
}
@media only screen and (max-width: 479px) {
.home{
	width:320px;
}
#after_header{
  width: 320px;
}
#header{
   width: 320px; 
}
#hr{
  width:320px;
}
#header_menu2{
  display:none;
}
#header_menu3{
  display:flex;
  padding-bottom:16px;
  display: flex;
  justify-content: center;
  align-items: center;
  color:#c6c6c7;
}
#after_header{
  display:none;
}
#after_header3{
  display:block;
}
.grig_part{
  display:block;
}
.img_padd{
  padding-top:15px;
}
#input_field{
  display:block;
}
.exp_part{
  margin-top:10px;
  width:100%;
  text-align: left;
  font-size: 12px;
  color:#FFFFFF
}
.exp_parts{
  padding:4px 20px;
  
}
.exp_parts:hover{
  opacity:0.7
  
}
.text_middle{
  display:none;
}
.gray_part{
  margin-bottom: 40px;
}
}
</style>

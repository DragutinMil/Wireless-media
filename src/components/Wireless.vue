<template>
  <div class="home">
    <div id="header">
      <img src="../assets/WMv1_04.jpg" id="logo"  alt="">   
      <div id="header_menu">
         <p> HOME </p> &nbsp;&nbsp;<p> /</p>&nbsp;&nbsp;
         <p> ABOUT US </p> &nbsp; &nbsp;<p> /</p>&nbsp;&nbsp;
         <p> OUR WORK </p> &nbsp;&nbsp;<p>/</p>&nbsp;&nbsp;
         <p> CONTACT </p> &nbsp;&nbsp;
      </div>
      <div id="header_menu2">
         <img src="../assets/novo_03.jpg" alt="">
         <img src="../assets/novo_05.jpg" alt="">
         <img src="../assets/novo_07.jpg" alt="">
         <img src="../assets/novo_09.jpg" alt="">
      </div>
      <div id="header_menu3">
         <img src="../assets/WMv99999_03.jpg" alt="">
      </div>
      <img id="search_icon" src="../assets/WMv1_13.jpg" alt="">

    </div>
	<img id="hr" src="../assets/WMv13333_06.jpg"  alt=""> 
	<img src="../assets/WMv13333_08.jpg" id="after_header"  alt=""> 
	<div>
		<h1>WHO WE ARE</h1>
	</div>
	<div class="grig_part">
		<div>
		<img src="../assets/WMv13333_12.jpg" id=""  alt=""> 
		</div>
		<div>
			<h3>Lorem ipsum</h3>
      <p class="text_middle">
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. 
      Distinctio mollitia rerum laudantium culpa.
      </p>
			<img class="show_button" src="../assets/WMv13333_15.jpg" alt="">
		</div>
	</div>
  <div class="grig_part">
     <div>
    <img src="../assets/WMv13333_19.jpg" id=""  alt=""> 
	</div>
	<div>
    <h3>Lorem ipsum </h3>
	  <p class="text_middle">
      Lorem ipsum dolor, sit amet consectetur adipisicing elit. 
    </p>
	  <img  class="show_button"
    src="../assets/WMv13333_15.jpg" 
    alt="" > 
	</div> 
  </div>
  <div>
		<h1>WHAT WE DO</h1>
	</div>
	<div>
    <div class="grig_part">
		  <div>
		    <img src="../assets/WMv13333_23.jpg" id=""  alt=""> 
	  	</div>
		  <div>
	    	<img src="../assets/WMv13333_22.jpg" id=""  alt=""> 
		  </div>
  	</div>
  </div>
  <div>
    <div class="grig_part">
		  <div>
		    <img src="../assets/WMv13333_26.jpg" id=""  alt=""> 
	  	</div>
		  <div>
	    	<img src="../assets/WMv13333_27.jpg" id=""  alt=""> 
		  </div>
  	</div>
  </div>
  <footer>
     <div>
      <img src="../assets/WMv1_50.jpg" alt="">
      <img src="../assets/WMv1_51.jpg" alt="">
      <img src="../assets/WMv1_52.jpg" alt="">
     </div>
     <div id="footer_menu">
         <p> HOME </p> &nbsp;&nbsp;&nbsp;&nbsp;
         <p> ABOUT US </p> &nbsp; &nbsp;&nbsp;&nbsp;
         <p> OUR WORK </p> &nbsp;&nbsp;&nbsp;&nbsp;
         <p> CONTACT </p> &nbsp;&nbsp;
      </div>
      <div>
        <img src="../assets/WMv1_59.jpg" alt="">
      </div>
  </footer>
  </div>
</template>

<script>
export default {
  name: 'Wireless',
  props: {
  }
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
.text_middle{
  color:#9e9e9d;
}
.home{
	margin:auto;
	width:765px;
}
.grig_part{
  padding:20px 10%;
  display:grid;
  grid-template-columns: 45% 45%;
  gap:10%;
}
.show_button{
  margin-left:50%
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
}
#header_menu{
  display: flex;
  justify-content: center;
  align-items: center;
  padding-bottom:10px;
  color:#c6c6c7;
  font-size: 18px;
  cursor: pointer;
}
#header_menu2{
  display:none;
}
#header_menu3{
  display:none;
}

#footer_menu{
  display: flex;
  justify-content: center;
  align-items: center;
  padding-bottom:10px;
  color:#858585;
  font-size: 18px;
  cursor: pointer;
}

#search_icon{
  height: 30px;
  padding-top:15px;
  padding-right:10px;
  cursor: pointer;
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
}
</style>

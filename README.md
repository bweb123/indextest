<!DOCTYPE html>
<html>
<head>
	<title></title>
	<link rel="stylesheet" href="style.css">
	<meta name="viewport" content="width=device-width">
	<style type="text/css">
		main{
	margin-left:6%;
	width: 100%;
	display: grid;
	align-items: center;
	text-align: center;
	grid-template-columns: 45% 45%;
	grid-template-rows: auto;
	grid-template-areas: 
	"title title"
	"one two"
	"three three"
}
#title{
	grid-area: title;
}
#one{
	grid-area: one;
}
#two{
	grid-area: two;
}
#three{
	grid-area: three;
}
@media only screen and (max-width: 700px){
main{
		margin-left:10%;
		width: 90%;
		display: grid;
		align-items: center;
		text-align: center;
		grid-template-columns: 45% 45%;
		grid-template-rows: auto;
		grid-template-areas: 
		"title title"
		"one one"
		"two two"
		"three three"
	}
	#title{
		grid-area: title;
	}
	#one{
		grid-area: one;
	}
	#two{
		grid-area: two;
	}
	#three{
		grid-area: three;
	}
	.main{
		margin-top: 3vh;
		border: 1px solid #fff;
		transition:  0.7s ease;
		padding: 2vh 2vh;
	}
	}
	</style>
</head>
<body>
	<div class="container">
		<div class="navbar">
			<img src="logo-white.png" class="logo">
			<nav>
				<ul id="menuList">
					<li id="active"><a href="index.html">Home</a></li>
					<li><a href="create_e-card.html">Create E-Card</a></li>
					<li><a href="aboutus.html">About Us</a></li>
					<li><a href="contact.html">Contact</a></li>
				</ul>
			</nav>
			<img src="menu.png" class="menu-icon" onclick="togglemenu()">
		</div>

		<main>
			<div id="title">
				<h1>Welcome To "e-invitation card"</h1>
				<h5>where you can create your own e-card for free!</h5>
			</div>
					<a id="one" href="#">
						<div class="main">
							<h1>Gallery</h1>
							<img src="logo-black.png">
						</div>
					</a>

					<a id="two" href="create_e-card.html">
						<div class="main" >
							<h1>Make Your Card</h1>
							<img src="logo-black.png">
						</div>
					</a>

					<a id="three" href="#">
						<div class="main" >			
							<h1>Tutorial On Making Your Own Card</h1>
						</div>
					</a>
		</main>
	</div>

	<script type="text/javascript">
		var menuList = document.getElementById("menuList");

		menuList.style.maxHeight = "0px";

		function togglemenu(){

			if(menuList.style.maxHeight == "0px"){
				menuList.style.maxHeight = "130px";
			}
			else{
				menuList.style.maxHeight = "0px";
			}
		}

	</script>

</body>
</html>


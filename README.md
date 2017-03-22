<html>
<head>
	<title>JSON Parse Stringify</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
	<script>
	$(document).ready(function(){
        
        $("button").click(function() {
        	//var infoStuff = document.getElementById("infostuff");
            //var obj = JSON.parse(infoStuff)
  			var obj = JSON.parse('{ "name":"John", "age":37, "city":"New York"}');
document.getElementById("box1").innerHTML = obj.name + ", " + obj.age + ", " +obj.city;
		});
	});
    
   
    
	</script>
	<style>
	body{
		background-color: rgb(90,120,250);
	}
	h1 {
		color: white;
	}
	p {
    	
		color:white;
	}
	#box1 {
		border:2px solid white;
        height:40px;
        padding:5px;
        width:275px;
        text-align:center;
	}
    
    button {
    	border-radius:3px;
        height:23px;
        width:70px;
        background-color:silver;
        margin-top:6%;
        margin-left:15%;
    }
	</style>
</head>
<body>

	

	<h1>Client Info:</h1>
    
	<p id="infostuff"> "name":"John", "age":37, "city":"New York"</p>
	<button>Parse</button>
	<div id="box1"></div>
	<section id="result_display"></section>
</body>
</html>

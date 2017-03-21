<html>
<head>
	<title>JSON Parse Stringify</title>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
	<script>
	$(document).ready(function(){
        
        $("button").click(function() {
  			var nome = document.getElementById('objName');
           
           document.write("New Client: " + nome.value + " #: " + num.value + " Area Code: "  + code.value + " Business: " + bus.value);
           
		});
	});
    
    var obj = JSON.parse('{ "name":"John", "age":37, "city":"New York"}');
document.getElementById("demo").innerHTML = obj.name + ", " + obj.age + ", " +obj.city;
    
	</script>
	<style>
	body{
		background-color: rgb(90,120,250);
	}
	h1 {
		color: white;
	}
	p {
    	margin-left:50%;
		color:white;
	}
	box1 {
		height: 70px;
		width: 70px;
		border: 10px solid red;
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
    
	<p></p>
	<button>Parse</button>
	<div id="box1"></div>
	<section id="result_display"></section>
</body>
</html>

<!DOCTYPE html>
	<html>
	<head>
	<meta charset="utf-8">
	<link rel="icon" href="https://cdn-icons-png.flaticon.com/512/252/252035.png">
	<title>Weather Info</title>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width" initial-scale=1>
	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
	<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.8.1/font/bootstrap-icons.css">
	<style type="text/css">
	body{
	background-image: url(https://media.istockphoto.com/photos/graduated-blue-summer-sky-genuine-photograph-picture-id1138440263?b=1&k=20&m=1138440263&s=170667a&w=0&h=EkMXQJvyUo5sLphvrZOREehPr4b9sVzrUaVxPM91eek=);
	background-repeat: no-repeat;
	background-size: 100%;
	}
	.loc{
	color: #072f88;
	font-family: initial;
	}
	.loc1{
	color: #f7fbfe;
	}
	</style>
	</head>
	<body>
	<div align="center" class="mt-3 loc"><h2>Location :<i class="loc1"> <%= location %></i></h2> </div>
	
	<div class="container mt-3" style="box-shadow: 0 2px 10px rgba(0,0,200,0.3); height: 450px;width: 400px;" align="text-center">
	
	<h3 class="loc">Region:<i class="loc1"> <%= region %></i></h3>
	<h3 class="loc">Country:<i class="loc1"> <%= country %></i></h3>
	<h3 class="loc">Local Time:<i class="loc1"> <%= loctime %></i></h3>
	<h3 class="loc">Temperature: <i class="loc1"><%= temp_c %><span>&#176;</span>C / <%= temp_f %><span>&#176;</span>F</i></h3>
	<h3 class="loc">Wind Speed:<i class="loc1"> <%= wind_kph %>KPH</i></h3>
	<h3 class="loc">Humidity:<i class="loc1"> <%= humi %></i></h3>
	<h3 class="loc">Feels like:<i class="loc1"> <%= feels_c %><span>&#176;</span>C / <%= feels_f %><span>&#176;</span>F</i></h3>
	<h3 class="loc">Condition: <i class="loc1"><%= condition %><img src="<%= icon %>"></i></h3>
	<div align="center">
	<form action="/locsubmit" method="GET"><button class="btn btn-primary" type="submit">Go Back</button></form></div>
	</div>
	</body>
	</html>

### Card-3D-with-Html-and-Css
#### Enjoy coding with html and css...

លំហាត់ខាងក្រោមនេះ ទាមទារឲ្យអ្នកមានចំណេះដឹងទាក់ទងនឹង:
- HTML
- CSS
  - Position
  - Transform 2D and 3D
  - Flexbox

# លំហាត់ Card 3D
![Thumbnail](/images/1.jpg)
# កូដ HTML:
```javascript
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<title>Card 3d</title>
	<!-- Css -->
	<link rel="stylesheet" type="text/css" href="css/style2.css">
	<!-- Google Font -->
	<link rel="preconnect" href="https://fonts.gstatic.com">
	<link href="https://fonts.googleapis.com/css2?family=Ubuntu:wght@300&display=swap" rel="stylesheet">
	<link rel="preconnect" href="https://fonts.gstatic.com">
	<link href="https://fonts.googleapis.com/css2?family=Preahvihear&family=Ubuntu:wght@300&display=swap" rel="stylesheet">
	<link rel="preconnect" href="https://fonts.gstatic.com">
	<link href="https://fonts.googleapis.com/css2?family=Content&family=Preahvihear&family=Ubuntu:wght@300&display=swap" rel="stylesheet">
</head>
<body>
	<div class="card">
		<div class="image">
			<img src="images/heng-visal.jpg" alt="heng visal">
		</div>
		<div class="content">
			<h3 class="title">
				<span class="eng">Heng Visal</span>
				 - 
				<span class="kh-title">ហេង វិសាល</span>
			</h3>
			<p class="paragraph kh">
				កុំសួរខ្ញុំថាស្អីគេស្នេហា រាល់ថ្ងៃស្គាល់តែបុិចនិងសៀវភៅទេ។​ ស្នេហាធ្វើឲ្យមនុស្សថោកទាប អានសៀវភៅទៅទើបល្។​ សម្រាប់ខ្ញុំ ស្នេហាវាធ្វើឲ្យខ្ញុំថោកទាប ព្រោះយើងបារម្ភគិតពីគេ ទោះបីជាគេមិនខ្វល់ក៏នៅតែបារម្ភ នៅតែគិត ទោះបីជាគេមិនចង់ជួប ក៏ខំត្រដរទៅជួប។
			</p>
			<p class="small-title kh">
				<small>(១)</small>
			</p>
		</div>
	</div>
</body>
</html>
```
# កូដ CSS:
```javascript
body{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	height: 100vh;
	display: flex;
	justify-content: center;
	align-items: center;
	background-color: #186A3B;
}

.eng{
	font-family: 'Ubuntu', sans-serif;
}

.kh-title{
	font-family: 'Preahvihear', cursive;
}

.kh{
	font-family: 'Content', cursive;
}

.card{
	width: 300px;
	height: 400px;
	background-color: #fff;
	transform-style: preserve-3d; 
	transform: perspective(2000px);
	transition: all 0.5s linear;
	position: relative;
	box-shadow: inset 300px 0 50px rgba(0,0,0,0.5); 
}

.card:hover{
	transform: perspective(2000px) rotate(-10deg);
	box-shadow: inset 20px 0 50px rgba(0,0,0,0.5);
}

.card .image{
	width: 100%;
	height: 100%;
	transform-origin: left;
	transition: all 0.5s linear;
	position: absolute;
	top: 0;
	left: 0;
	z-index: 10;
	cursor: pointer;
	border: 1px solid #333;
}

.card:hover .image{
	transform: rotateY(-140deg);
}

.card .image > img{
	width: 100%;
	height: 100%;
	object-fit: cover;
}

.card .content{
	position: absolute;
	top: 0;
	left: 0;
	padding: 20px 40px;
	text-align: center;
}

.card .content .paragraph{
	margin-bottom: -10px;
}
```
[Facebook-MengSreang Channel](https://www.facebook.com/mengsreangchannel)

[Facebook-CodeIsMine](https://www.facebook.com/CodeIsMine)

[YouTube-MengSreang Channel](https://www.youtube.com/channel/UCE6UmKNi-bYNWwOBUYoT-yQ)

[YouTube-CodeIsMine](https://www.youtube.com/channel/UCBKsUkGih9kdXcrz54zNH1w)

### អរគុណច្រើន សំណាងល្អ!🙏

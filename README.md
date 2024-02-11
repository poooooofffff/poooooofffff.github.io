<html>
	<head>
		<title>
		Be My Valentine?
		</title>

		<script type="text/javascript">

			function yesClicked() {
				document.write('<title>Romnick said Yes!</title>');
				document.write('\
					<style>\
  						footer {\
    							position: fixed;\
    							bottom: 0;\
    							right: 0;\
    							padding: 10px;\
    							text-align: left;\
    							font-size: 10px;\
    							line-height: 0.5;\
  						}\
					\
					h1 {\
						color: #FF8096;\
					}\
					</style>\
				\
					<center>\
						<h1><br>YEEEYYY!!!</h1><br><br>\
						<img src="gif2.gif" alt="GIF Description"><br><br>\
						<p>I love you beehhhh</p>\
					</center>\
				\
					<footer>\
  						<p><b>From your boyfriend, David Northrup :3</b></p>\
					</footer>\
				');
			}

			function showCustomAlert() {
				var alertBox = document.getElementById('customAlert');
            alertBox.style.display = 'block';
            alertBox.classList.remove('hide');
			}

			function closeAlert() {
				var alertBox = document.getElementById('customAlert');
				alertBox.classList.add('hide');
			}
		</script>
	</head>

	
	<body>
		<style>
  			footer {
    			position: fixed;
    			bottom: 45px;
    			right: 0;
    			padding: 10px;
    			text-align: left;
    			font-size: 10px;
				line-height: 0.5;
  			}
			
			h1 {
				color: #FF8096;
			}

			button {
    			background-color: #FF8096;
    			color: white;
    			padding: 10px 20px;
    			border: none;
    			border-radius: 5px;
    			cursor: pointer;
				width: 20%;
  			}

  			button:hover {
    			background-color: #E30B5C;
  			}
			
			.alert {
				display: none;
				padding: 20px;
				background-color: #f44336;
				color: white;
				position: fixed;
				bottom: 0;
				left: 0;
				right: 0;
				animation: swipeUp 1.5s ease;
			}
			
			.alert.hide {
				animation: swipeDown 1.5s ease forwards;
			}

			@keyframes swipeUp {
				from {
					bottom: -70;
				}
				to {
					bottom: 0;
				}
			}
			
			@keyframes swipeDown {
				from {
					bottom: 0;
				}
				to {
					bottom: -70;
				}
			}

			.closebtn {
				margin-left: 15px;
				color: white;
				font-weight: bold;
				float: right;
				font-size: 22px;
				line-height: 20px;
				cursor: pointer;
				transition: 0.3s;
			}

			.closebtn:hover {
				color: black;
			}
		</style>

		<center>
			<h1><br>Will you be my Valentine?</h1>
			<hr size="4" width="100%" color="#FF8096"><br>
			
			<button onclick="yesClicked()">
			Yes</button>
			
			<button onclick="showCustomAlert()">
			No</button><br><br>
			
			<img src="gif1.gif" alt="GIF Description">
			
			<div id="customAlert" class="alert">
				<span class="closebtn" onclick="closeAlert()">&times;</span> 
				<b>Oops! An error occurred: </b> Unable to save user input. Dapat ang "Yes" jud ang pilion nimo beh.
			</div>
		</center>

		<footer>
			<p><b>From your boyfriend, David Northrup :3</b></p>
		</footer>
	</body>

</html>

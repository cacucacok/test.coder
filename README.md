<!DOCTYPE html>
<html>
<head>
	<title>Random Image Generator</title>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
	<h1>Random Image Generator</h1>
	<p>Click the button to generate a random image:</p>
	<button onclick="generateImage()">Generate</button>
	<img id="result" src="" alt="">

	<script>
		function generateImage() {
			var images = [
				"https://picsum.photos/200/300",
				"https://picsum.photos/250/400",
				"https://picsum.photos/300/500",
				"https://picsum.photos/350/550",
				"https://picsum.photos/400/600"
			];
			var image = images[Math.floor(Math.random() * images.length)];
			document.getElementById("result").src = image;
		}
	</script>
</body>
</html>

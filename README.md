<html>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="/w3css/3/w3.css">
<body>

<!-- Navigation -->
<nav class="w3-bar w3-black">
  <a href="#home" class="w3-button w3-bar-item">Home</a>
  <a href="#chat" class="w3-button w3-bar-item">Chat</a>
  <a href="#share" class="w3-button w3-bar-item">Share</a>
  <a href="#contact" class="w3-button w3-bar-item">Contact</a>
</nav>

<!-- Slide Show Legg til bilde -->
<section>
  <img class="mySlides" src="http://i0.kym-cdn.com/photos/images/newsfeed/001/344/654/45b.png"
  style="width:100%">
  <img class="mySlides" src="https://orig00.deviantart.net/3d50/f/2013/128/3/6/stahp_it_by_wsmarkhenry-d64lpx9.jpg"
  style="width:100%">
  <img class="mySlides" src="https://cdn-images-1.medium.com/max/1440/1*Sn80dgiwpMjBVrqjfiDbnA.jpeg"
  style="width:100%">
</section>

// Automatic Slideshow - change image every 3 seconds
var myIndex = 0;
carousel();

function carousel() {
    var i;
    var x = document.getElementsByClassName("mySlides");
    for (i = 0; i < x.length; i++) {
        x[i].style.display = "none";
    }
    myIndex++;
    if (myIndex > x.length) {myIndex = 1}
    x[myIndex-1].style.display = "block";
    setTimeout(carousel, 3000);
}

</body>
</html>

<!DOCTYPE html>
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
  <img class="mySlides" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTRff7tt8jNJ4SlkQsVf37_KBG3MK1NdhXpUgLNrVL7yhEuWwWo"
  style="width:100%">
  <img class="mySlides" src="HER"
  style="width:100%">
  <img class="mySlides" src="HER"
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

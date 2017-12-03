---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# layout: home
layout: default
title: Home
---

**AnATLyzer** is a static analyser for ATL, available as an extension of the ATL IDE. 

 <div class="slideshow-container">
  <div class="mySlides fade">
    <div class="numbertext">1 / 3</div>
    <img src="{{ site.baseurl }}public/images/anatlyzer_screenshot.png" style="width:100; max-width: 600px">
    <!--
    <div class="text">AnATLyzer showing errors</div>
    -->
  </div>

  <div class="mySlides fade">
    <div class="numbertext">2 / 3</div>
    <img src="{{ site.baseurl }}public/images/visualization.png" style="width:100; max-width: 600px">
    <!--
    <div class="text">Visualizations</div>
    -->
  </div>

  <div class="mySlides fade">
    <div class="numbertext">3 / 3</div>
    <img src="{{ site.baseurl }}public/images/witness_model.png" style="width:100; max-width: 600px">
    <!--
    <div class="text">Generation of example models</div>
    -->
  </div>

  <a class="prev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span>
  <span class="dot" onclick="currentSlide(2)"></span>
  <span class="dot" onclick="currentSlide(3)"></span>
</div> 

<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active_slide", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active_slide";
} 
</script>

<!--
<div class="slider-holder">
        <span id="slider-image-1"></span>
        <span id="slider-image-2"></span>
        <span id="slider-image-3"></span>
        <div class="image-holder">
            <img height="400" src="{{ site.baseurl }}public/images/anatlyzer_screenshot.png" class="slider-image" />
            <img height="400" src="{{ site.baseurl }}public/images/visualization.png" class="slider-image" />
            <img height="400" src="{{ site.baseurl }}public/images/witness_model.png" class="slider-image" />
        </div>
        <div class="button-holder">
            <a href="#slider-image-1" class="slider-change"></a>
            <a href="#slider-image-2" class="slider-change"></a>
            <a href="#slider-image-3" class="slider-change"></a>
        </div>
</div>
-->


<p></p>

AnATLyzer has a number of features intended to increase the correctness of the transformations and the productivity of the model transformation developers:

* Static typing of the ATL programs
* Detection of more than 50 kinds of problems
* Error markers and a special analysis view
* Support for pre-conditions and post-conditions
* A large catalogue of quick fixes
* Visualizations of rule relationships
* Integration with the standard ATL editor
* A programmatic API to easily manipulated typed ATL programs


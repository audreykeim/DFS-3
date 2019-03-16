# DFS-3
<div class= "circle"></div>
<div class= "circle2"></div>
<style
  .circle{
    background: red;
    width: 100px;
    height: 100px;
    border-radius: 50%;
  position : absolute;
  }
  .word{
  color: blue;
  position: absolute;
}

var circle = $(".circle");
console.log(circle[0].offsetHeight);
$( document ).on( "mousemove", function( event ) {
  $( "#log" ).text( "pageX: " + event.pageX + ", pageY: " + event.pageY ); console.log("bingo");
var screenWidth = $( document ).width();
var cursorX = event.pageX;
var cursorY = event.pageY;
var opacity = (screenWidth - cursorX) / screenWidth ;
  $(".circle").css({
  "opacity": opacity,
  "left": cursorX,
  "top": cursorY})
 });

var word = $(".word");
console.log(word[0].offsetHeight);
$( document ).on( "mousemove", function( event ) {
  $( "#log" ).text( "pageX: " + event.pageX + ", pageY: " + event.pageY ); console.log("bingo");
var screenWidth = $( document ).width();
var cursorX = event.pageX;
var cursorY = event.pageY;
var opacity = (screenWidth - cursorX) / screenWidth ;
  $(".word").css({
  "opacity": opacity,
  "right": cursorX,
  "top": cursorY})
 });


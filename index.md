<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>

*{margin: 0px;
  padding: 0px;}

body{
  background-color: black;
}

p {
  font-size: 60px;
  align-self: center;
  color: white;
}

#wrapper{
  display: flex;
  justify-content: center;
  height: 100%;
  width: 100%;
}

</style>
</head>
<body>

<div id="wrapper">
<p id="demo"></p>
</div>

<script>
// Set the date we're counting down to
var countDownDate = new Date("June 07, 2020 20:00:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

  // Get today's date and time
  var now = new Date().getTime();
    
  // Find the distance between now and the count down date
  var distance = countDownDate - now;
    
  // Time calculations for days, hours, minutes and seconds
  var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);
    
  // Output the result in an element with id="demo"
  document.getElementById("demo").innerHTML = days + "d " + hours + "h "
  + minutes + "m " + seconds + "s ";
    
  // If the count down is over, write some text 
  if (distance < 0) {
    clearInterval(x);
    document.getElementById("demo").innerHTML = "relikairmp.github.io/showtime";
  }
}, 1000);
</script>

</body>
</html>
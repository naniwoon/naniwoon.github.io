# naniwoon.github.io
<html>
  <head>
    <link rel="stylesheet" href="index.css" />
    <script src="jquery-3.2.1.js"></script>
    <title>My Website</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta property="og:locale" content="en_US">
    <meta property="og:type" content="website">
    <meta property="og:title" content="My Portfolio">
    <meta property="og:description" content="Built with Next Academy">
    <meta property="og:site_name" content="My Portfolio">
    <meta property="og:image" content="https://www.nextacademy.com/img/share/nextacademy-generic.jpg">
  </head>
  <body>
    <div id="navbar">
      <a href="#about" class="nav-links">Go To About Me </a>
      <a href="#show" class="nav-links">My Past Experience </a>
      </div>

    <div class="container">
      <div class="small-container" id="about">
        <h5>Hello, I'm Tiong Woon.</h5>
        <p>This is my first website, </p>
        <p>  and I'm interested in coding.</p>
        <p>I'm from Earth and I love music.</p>
        <p>This is how I look chill. </p>
        <img src="Picture2.png">
      </div>

      <div class="small-container" id="show">
        <h1>What I've done in the past</h1>
        <ul>
          <li id="special"> Learn to code</li>
          <li>Some digital marketing</li>
          <li>Travel</li>
        </ul>
        <a href="https://www.nextacademy.com">
          Learn to code from Next Academy
        </a>
      </div>

      <div class="small-container">
        <button id="surprise-button">CLick me for surprise!</button>
        <div id="haha"></div>
    </div>

  </div>
  </body>
  <script>
  $(document).ready(function() {
    $("#surprise-button").click(function(e) {
      $.get("http://api.giphy.com/v1/gifs/random?tag=trumph&api_key=dc6zaTOxFJmzC", function(res) {
        $('#haha').html('<img src="' + res.data.image_url + '">' )
      })
    })
  })
</script>
</html>

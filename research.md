<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
  
* {
  box-sizing: border-box;
}

.column {
  float: left;
  width: 33.33%;
  padding: 5px;
}

/* Clearfix (clear floats) */
.row::after {
  content: "";
  clear: both;
  display: table;
}

.container {
  position: relative;
  width: 100%;
}

.image {
  display: block;
  width: 100%;
  height: auto;
}

.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: #2AAD95;
}

.container:hover .overlay {
  opacity: 1;
}

.text {
  color: white;
  font-size: 16px;
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}

/* Expandable text container */
.content {
  position: relative;
  padding: 0 12px;
  display: none;
  overflow: hidden;
  background-color: #f1f1f1;
}

/* Closable button inside the image */
.closebtn {
  position: absolute;
  top: 10px;
  right: 15px;
  color: white;
  font-size: 35px;
  cursor: pointer;
}

</style>
</head>
<body>

<h3>Current Projects</h3>

<div class="row">
  <div class="column">
    <div class="container">
      <img src="/images/ffint.png" alt="ffint" class="image">
      <div class="overlay">
        <div class="text">Changing Stiffness by Wing Morphing</div>
      </div>
    </div>
    <div class="content">
      <p>Lorem ipsum...</p>
    </div>
  </div>
  <div class="column">
    <div class="container">
      <img src="/images/Q criterion.png" alt="cfd" class="image">
      <div class="overlay">
        <div class="text">FSI Modelling</div>
      </div>
    </div>
    <div class="content">
      <p>Lorem ipsum...</p>
    </div>
  </div>
  <div class="column">
    <div class="container">
      <img src="/images/feathers.JPG" alt="momocs" class="image">
      <div class="overlay">
        <div class="text">Feather Asymmetry</div>
      </div>
    </div>
    <div class="content">
      <p>Lorem ipsum...</p>
    </div>
  </div>
</div>

<h3>Past Projects</h3>

<div class="row">
  <div class="column">
    <div class="container">
      <img src="/images/sliposi.png" alt="aorta" class="image" onclick="myFunction(this);">
      <div class="overlay">
        <div class="text">Multi-scale Haemodynamics</div>
      </div>
    </div>
    <div class="content">
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna       aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
    </div>
  </div>
</div>

<!-- The expanding image container -->
<div class="content">
  <!-- Close the image -->
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>

  <!-- Expanded content -->
  <img id="expandedcontent" style="width:100%">

</div>

function myFunction(imgs) {
  // Get the expanded content
  var expandcontent = document.getElementById("expandedcontent");
  // Use the same src in the expanded image as the image being clicked on from the grid
  expandImg.src = imgs.src;
  // Show the container element (hidden with CSS)
  expandImg.parentElement.style.display = "block";
} 

<!--
<script>
var coll = document.getElementsByClassName("container");
var i;
for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.display === "block") {
      content.style.display = "none";
    } else {
      content.style.display = "block";
    }
  });
}
</script> -->

</body>
</html>

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
  width: 100%;
}

</style>
</head>
<body>

<h3>Current Projects</h3>

<!-- Buttons -->
<div class="row">
  <div class="column">
    <div class="container">
      <img src="/images/ffint.png" alt="ffint" class="image">
      <div class="overlay">
        <div class="text">Changing Stiffness by Wing Morphing</div>
      </div>
    </div>
  </div>
  <div class="column">
    <div class="container">
      <img src="/images/Q criterion.png" alt="cfd" class="image">
      <div class="overlay">
        <div class="text">FSI Modelling</div>
      </div>
    </div>
  </div>
  <div class="column">
    <div class="container">
      <img src="/images/feathers.JPG" alt="momocs" class="image">
      <div class="overlay">
        <div class="text">Feather Asymmetry</div>
      </div>
    </div>
  </div>
</div>

<h3>Past Projects</h3>

<div class="row">
  <div class="column">
    <div class="container">
      <img src="/images/sliposi.png" alt="aorta" class="image" onclick="myFunction(event, 'aorta')">
      <div class="overlay">
        <div class="text">Multi-scale Haemodynamics</div>
      </div>
    </div>
  </div>
</div>
  
<!-- content -->
<div id="ffint" class="content">
  <h3>FFINT</h3>
  <p>Wing folding increases feather anchoring stiffness near joints.</p>
</div>
<div id="cfd" class="content">
  <h3>FSI</h3>
  <p>Increasing tissue stiffness... </p>
</div>
<div id="feamorph" class="content">
  <h3>Feather Morphology</h3>
  <p>Assymmetry increases towards to distal wing.</p>
</div>
<div id="aorta" class="content">
  <h3>Multi-scale Haemodynamics</h3>
  <p>Endothelial cell shape change affects local measurements of wall shear stress.</p>
</div>

<script>
function myFunctiony(evt, proj) {
  var i, content, container;
  content = document.getElementsByClassName("content");
  for (i = 0; i < content.length; i++) {
    content[i].style.display = "none";
  }
  container = document.getElementsByClassName("container");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = container[i].className.replace(" active", "");
  }
  document.getElementById(proj).style.display = "block";
  evt.currentTarget.className += " active";
}

</body>
</html>

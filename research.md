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
      <img src="/images/sliposi.png" alt="aorta" class="image">
      <div class="overlay">
        <div class="text">Multi-scale Haemodynamics</div>
      </div>
    </div>
  </div>
</div>

</body>
</html>

<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
  
.collapsible {
  background-color: #7D9994;
  color: white;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: 1px solid #000000;
  border-radius: 10px;
  text-align: left;
  outline: 1px solid #000000;
  outline-radius: 10px;
  font-size: 15px;
}

.active, .collapsible:hover {
  background-color: #004d4d;
}

.content {
  padding: 2px 18px;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
  background-color: #f1f1f1;
}
</style>
</head>
<body>

<h3>Current Projects</h3>

<button class="collapsible">Morphological signal processing of flow information in a morphing wing</button>
<div class="content">
  <br>
  <p>Birds have vibration-sensitive mechanoreceptors embedded throughout the wing tissue in the leading edge. Flow over the wing will deform the feathers and this vibration signal must then be transferred throughout the feathered array to these mechanoreceptors. This project looks at how different flows result in different vibration responses in the wing, and how those responses are processed by the feathers throughout wing morphing. </p>
</div>

<button class="collapsible">Wing morphing-induced effects on aeroelastic responses during gliding flight</button>
<div class="content">
  <br>
  <p>Wing morphing induces the rearrangement of a multi-material, multi-component feathered structure to effect a shape change. This project quantifies the associated changes in <i>in situ</i> mechanical properties and then makes use of fluid-structure interaction numerical methods to explore how coupling changes in stiffness to wing morphing change the aeroelastic responses to gliding flight at different speeds.</p>
</div>

<button class="collapsible">Interspecific variation in feather structure</button>
<div class="content">
  <br>
  <p>Feather shape varies within a wing and between species. We use geometric morphometrics methods to identify main axes of variation in these feathers from over 20 different species of birds and explore how shape variation is related to flight. </p>
</div>

<button class="collapsible">Zebra finch learning during flap-bounding flight</button>
<div class="content">
  <br>
  <p>In a collaboration with Dr Clementine Bodin and Dr Sarah Woolley at McGill University, we are exploring zebra finch learning behaviour in regards to flight and making use of optimisation analysis to postulate the motivation driving learned behaviour.</p>
</div>

<h3></h3>

<h3>Past Projects</h3>

<button class="collapsible">Multi-scale Modelling of Endothelial Cell Shape on Aorta Haemodynamics</button>
<div class="content">
  <br>
  <p>Wall shear stress (WSS) has been linked to the development of many cardiovascular diseases, including atherosclerosis and aneurysms. The pathology of these diseases is dictated by biological processes regulated by shear-sensitive endothelial cells (ECs) lining the blood vessel which morph in response to WSS signals. Computational fluid simulations used to study and identify vulnerable areas in the blood transport system have not yet accounted for this variable EC shape.</p>
    
  <p>To address this gap, we developped a computationally inexpensive multiscale algorithm to investigated the effects of microscopic EC morphology on WSS in macroscopic, realistic aorta models. The inclusion of EC geometry resulted in an increase of low time-averaged WSS and high oscillatory shear index (OSI) areas, and large differences in time-dependent WSS in cases with pathologically disturbed flow.</p>
  
  <p>For more details on the algorithm, see my thesis <a href="https://repository.hkust.edu.hk/ir/Record/1783.1-87034">here</a>.</p>
</div>

<script>
var coll = document.getElementsByClassName("collapsible");
var i;

for (i = 0; i < coll.length; i++) {
  coll[i].addEventListener("click", function() {
    this.classList.toggle("active");
    var content = this.nextElementSibling;
    if (content.style.maxHeight){
      content.style.maxHeight = null;
    } else {
      content.style.maxHeight = content.scrollHeight + "px";
    } 
  });
}
</script>

</body>
</html>

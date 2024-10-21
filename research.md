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
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
}

.active, .collapsible:hover {
  background-color: #004d4d;
}

.content {
  padding: 0px 18px;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.2s ease-out;
  background-color: #f1f1f1;
}
</style>
</head>
<body>

<h3>Current Projects</h3>

<button class="collapsible">Wing Morphing Induced Changes to Local Mechanical Properties</button>
<div class="content">
  <p> 
    The avian wing is unique in that all active morphing elements are concentrated at the leading edge while the majority of the flight surface is made up of passive, flexible elements. As active morphing changes the overall wing shape, how does the coupled rearrangement of these passive elements affect local stiffness and damping capabilities?</p>
</div>
<button class="collapsible">Effects of Wing Stiffness Change to Aeroelastic Responses</button>
<div class="content">
  <p>In flight, birds morph their wings to adjust to changing environmental conditions and behavioural goals. Wing morphing induces the rearrangement of a multi-material, multi-component structure resulting in changes in wing stiffness as well as a change in overall shape. Fluid-structure interaction computational modelling is used to explore how wing shape and coupled stiffness changes are beneficial or detrimental under different flight conditions.</p>
</div>
<button class="collapsible">Comparative Feather Morphology on Aerostructural Performance</button>
<div class="content">
  <p>Feather shape varies dramatically within a wing and between species. With data collected from over 20 species, we explore how individual feather shape, the spacing between them, and their orientation relative to the airflow can affect aeroelastic response and aerodynamic performance. </p>
</div>

<h3></h3>

<h3>Past Projects</h3>

<button class="collapsible">Multi-scale Modelling of Endothelial Cell Shape on Aorta Haemodynamics</button>
<div class="content">
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

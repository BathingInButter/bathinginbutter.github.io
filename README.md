<body style="background-color:black;">
<div class="quantity">
  <input type="number" class="input-box" value="0" min="0" max="999">
</div>

<div class="dropdown">
  <button onclick="myFunction()" class="dropbtn"></button>
  <div id="myDropdown" class="dropdown-content">
    <p>Add</p>
    <p>Subtract</p>
    .dropbtn {
  background-color: #3498DB;
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
  cursor: pointer;
}
    .dropbtn:hover, .dropbtn:focus {
  background-color: #2980B9;
    .dropdown {
  position: relative;
  display: inline-block;
      display: none;
  position: absolute;
  background-color: #f1f1f1;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
  z-index: 1;
    .dropdown-content p {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
    .show {display:block;}
    function myFunction() {
  document.getElementById("myDropdown").classList.toggle("show");
}
    window.onclick = function(event) {
  if (!event.target.matches('.dropbtn')) {
    var dropdowns = document.getElementsByClassName("dropdown-content");
    var i;
    for (i = 0; i < dropdowns.length; i++) {
      var openDropdown = dropdowns[i];
      if (openDropdown.classList.contains('show')) {
        openDropdown.classList.remove('show');
      }
    }
  }
}
  </div>

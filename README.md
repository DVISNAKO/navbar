# navbar
Responsive Navigation Bar №1
<br>
<br>
With Html, CSS, Javascript
<br>
<br>
![127 0 0 1_5500_index html# - Google Chrome 15 12 2022 16_46_23 (2)](https://user-images.githubusercontent.com/106438454/207890890-d39e61eb-7511-4561-a70f-f7d7f1171a26.png)
<BR>
JAVASCRIPT -> BUTTONS CHANGE TAB SCREEN 
<br>
<br>
IF SCREEN WILL BE > 500px <br>
![bar](https://user-images.githubusercontent.com/106438454/207892037-4267a73b-f978-460b-bdb3-cb000a94ce4c.png)

<BR>
CODE

<!-- Navbar with Icons -->
    <h2>Responsive Navigation Bar with Icons</h2>
    <div class="navbar">
        <a class="active" href="#"><i class="fa fa-fw fa-home"></i> Home</a>
        <a href="#"><i class="fa fa-fw fa-search"></i> Search</a>
        <a href="#"><i class="fa fa-fw fa-envelope"></i> Contact</a>
        <a href="#"><i class="fa fa-fw fa-user"></i> Login</a>
    </div>
    
----
    
    <!-- Icon bar -->
    <h2>Icon bar</h2>
    <div class="icon-bar">
        <a class="active" href="#"><i class="fa fa-home"></i></a>
        <a href="#"><i class="fa fa-search"></i></a>
        <a href="#"><i class="fa fa-envelope"></i></a>
        <a href="#"><i class="fa fa-globe"></i></a>
        <a href="#"><i class="fa fa-trash"></i></a>
    </div>
    
  -----
    
    <!-- Tab header -->
    <h2>Tab bar</h2>
    <div id="London" class="tabcontent">
        <h1>London</h1>
        <p>London is the capital city of England.</p>
    </div>

    <div id="Paris" class="tabcontent">
        <h1>Paris</h1>
        <p>Paris is the capital of France.</p>
    </div>

    <div id="Tokyo" class="tabcontent">
        <h1>Tokyo</h1>
        <p>Tokyo is the capital of Japan.</p>
    </div>

    <div id="Oslo" class="tabcontent">
        <h1>Oslo</h1>
        <p>Oslo is the capital of Norway.</p>
    </div>

    <!-- Javascript -->
    <button class="tablink" onclick="openCity('London', this, 'red')" id="defaultOpen">London</button>
    <button class="tablink" onclick="openCity('Paris', this, 'green')">Paris</button>
    <button class="tablink" onclick="openCity('Tokyo', this, 'blue')">Tokyo</button>
    <button class="tablink" onclick="openCity('Oslo', this, 'orange')">Oslo</button>
    <script>


        function openCity(cityName, elmnt, color) {
            var i, tabcontent, tablinks;
            tabcontent = document.getElementsByClassName("tabcontent");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
            }
            tablinks = document.getElementsByClassName("tablink");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].style.backgroundColor = "";
            }
            document.getElementById(cityName).style.display = "block";
            elmnt.style.backgroundColor = color;

        }

        document.getElementById("defaultOpen").click();     
    </script>
    
    
    

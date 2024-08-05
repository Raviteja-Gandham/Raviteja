
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Learn Hub Navbar</title>
    <link rel="stylesheet" href="navbar.css">
    <link rel="stylesheet" href="section1.css">
    <style>
        body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    scroll-behavior: smooth;
}
li{
        display: block;
        text-decoration: none;  
}
a{
    text-decoration: none;
    color: white;
}

.navbar {
    display: flex;
    align-items: center;
    padding: 10px 20px;
    background-color: black;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
.Cards{
    
    align-items: center;
    justify-content: center;
    
}
/*
.logo-container {
    display: flex;
    align-items: center;
    animation: spin 10s linear infinite;
}
*/
.logo {
    width: 50px;
    height: 50px;
    margin-right: 10px;
    border: 2px solid black;
    padding: 5px;
    
}

.logo img {
    cursor: pointer;
    width: 100%;
    height: 100%;
    display: block;
    position: relative;
    left: -100%; /* Start position off-screen */
    /*font-weight: bold;*/
    animation: moveFromLeft 2s forwards; /* 2s animation duration */
}

.image{
    display: flex;
    justify-content: end;
    align-items: center;
   /* position: relative; */
    background-color: darkseagreen;
    font-size: 2vw;
   }    
.Course-logos{
    /*position: absolute; */
    margin-top: 50%;
    height: 100%;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
}

.title {
    font-size: 1.5em;
    margin: 0;
    color: rgb(186, 186, 29);
    
    position: relative;
    left: -100%; /* Start position off-screen */
   /* font-weight: bold;*/
    animation: moveFromLeft 2s forwards; /* 2s animation duration */
}

.tagline {
    font-size: 0.9em;
    color: #555;
    margin: 0;
    color: rgb(186, 186, 29);
    position: relative;
    left: -100%; /* Start position off-screen */
   /* font-weight: bold;*/
    animation: moveFromLeft 4s forwards; /* 4s animation duration */
}

.menu {
    display: flex;
    margin-left: auto;
    list-style: none;
    padding: 0;
      
}

.menu-item {
    position: relative;
    margin: 0 20px;
    font-size: 1em;
    cursor: pointer;
}

.menu-item:hover .dropdown {
    display: block;
    background-color: black;
}

.dropdown {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    padding: 10px 0;
    z-index: 1;
}

.dropdown-item {
    padding: 10px 20px;
    white-space: nowrap;
}

.dropdown-item:hover {
    background-color: #2f2d2d;
}

.search-container {
    position: relative;
    display: flex;
    align-items: center;
    background-color: black;
}

.search-container input {
    padding: 5px 10px;
    border-radius: 15px;
    border: 1px solid #ddd;
    outline: none;
    transition: all 0.3s ease;
}

.search-container input:focus {
    border-color: #aaa;
}

.search-container .icon {
    position: absolute;
    right: 10px;
    cursor: pointer;
}/*
.Contact{
   padding: 5%;
   padding-left: 10%;
   padding-top: 3%;
   color: white;
}
.Contact-details{
    background-color: black;
}
*/
.contact {
    text-align: left;
    padding: 20px;
    background-color: black;
    color: white;
    padding-left: 10%;
}
.contact-details {
    margin-bottom: 10px;
}
.contact-details span{
    font-weight: bold;
}
.contact-details a:hover{
    color: pink;
    
}
.contact-details img {
    vertical-align: middle;
    margin-right: 10px;
}
.Mission{
    background-color: darkseagreen;
    padding-bottom: 0%; 
    display: flex;
}
 .Mission-item{
    background: antiquewhite;
    /*background-color: lightgreen;*/
    border-radius: 15px;
    padding: 20px;
    margin: 10%;
    width: 80%;
    height: auto;
    max-width: 600px;
    text-align: center;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);   
    position: relative;
}
 
.Services {
       background-color: darkseagreen;
} 
.Serv-item{
    padding-left: 40%;
    color: whit;
    background-repeat: no-repeat;
    background-size: cover;
    border: 2px solid black;
    border-radius: 10px;
    width: 50%;
    padding: 30px;
    margin-left: 20%;
    background-color: lightseagreen;
}
.Serv-item h2{
    padding-left: 40%;
    
}
    /*
    display: flex;
    margin: 30%;
    width: 100px;
    position: absolute;
    transform: rotate(90deg);
    
}*/
/*
@keyframes spin {
    from {transform: rotate(0deg);}
    to {transform: rotate(360deg);}
}*/
@keyframes moveFromLeft {
    0% {
        left: -100%;
    }
    100% {
        left: 0%;
    }
}
    </style>
</head>
<body>
    <nav class="navbar">
        <div class="logo-container">
            <div class="logo">
                <a href="navbar.html" target="_self"><img src="logo.png" alt="Logo"></a> <!-- replace with actual logo image -->
            </div>
        </div>
        <div>
            <h1 class="title">Learn Hub</h1>
            <p class="tagline">Let's learn together</p>
        </div>
        <ul class="menu">
            <li class="menu-item">
                <a href="C:\Ravi\htmlfiles\FEW_project_2024\login.html" target="_blank">Logout</a>              </li>
              <li class="menu-item" id="scroll_contact">
                <a href="#" target="">Contact</a>
              </li>

            <li class="menu-item" id="scroll_about">
               <a href="#"> AboutUs</a>
                <ul class="dropdown" id="target_about">
                    <li class="dropdown-item"><a href="#" id="target_about">Our Mission</a></li>
                    <li class="dropdown-item"><a href="#"  id="target_about">Our Team</a></li>
                </ul>
            </li>
            <li class="menu-item" id="scroll_service">
              <a href="#">Services</a>
            </li>
            <li class="menu-item">
                <a href="#">Courses</a>
                   <ul class="dropdown">
                       <li class="dropdown-item"><a href="htmlcontent1.html" target="_blank"> HTML</a></li>
                       <li class="dropdown-item"><a href="css1.html" target="_blank"> CSS</a></li>
                       <li class="dropdown-item"><a href="js1.html"> Java Script</a></li>
                   </ul>
               </li>
        </ul>
        <div class="search-container">
            <input type="text" placeholder="Search...">
            <span class="icon">🔍</span>
        </div>
    </nav>
<!--

<div class="cards">
    <h1>What can we do for you?</h1>
</div> -->
    <header>
        <div class="hero-section">
            <div class="hero-content">
                <h1>Unlock Your Potential with Learn Hub</h1>
                <p>Empower your future with our vast range of online courses, expert instructors, and flexible learning paths designed for your success.</p>
                <div class="cta-buttons">
                    <a href="#" class="btn btn-primary">Get Started</a>
                    <a href="#" class="btn btn-secondary">Explore Courses</a>
                </div>
            </div>
        </div>
    </header>
<!--
<div class="image">
    <div class="Quote">
  <h1 style="color: white; font-size: 2.5vw;"> It's teach you how to learn and grow for personal<br>
     as well as in professional manner</h1>
    </div> 
   <img src="C:\Ravi\htmlfiles\FEW_project_2024\navigationBar\learnboy.png" alt="html-logo">
-->
   <!--
<div class="Course-logos">
    <img src="C:\Ravi\htmlfiles\FEW_project_2024\navigationBar\html-logo.png" height="200vh" width="200vw" alt="html-logo">
       <img src="C:\Ravi\htmlfiles\FEW_project_2024\navigationBar\css-logo.png" height="200vh" width="200vw" alt="css-logo">
      <img src="C:\Ravi\htmlfiles\FEW_project_2024\navigationBar\js-logo.png" height="205vh" width="230vw" alt="js-logo">
</div>  -->
</div>
<div class="Mission" id="scroll_mission">
    <div class="Mission-item" id="target_mission">
    <h2>Our Mission</h2>
    <p>
        At Learn Hub, our mission is to empower individuals through accessible, 
        high-quality education. We believe that everyone deserves the opportunity to learn and grow, 
        regardless of their background or circumstances. By providing a diverse range of resources, 
        we aim to foster a lifelong love of learning and help our users achieve their personal and professional goals. 
        Together, we're building a brighter future, one learner at a time.
    </p>
    </div>
   <div class="Mission-item" style="background-color: antiquewhite;">
    <h2>Our Team</h2>
        <img src="team.jpg" alt="team" style="height: 300px; width: 300px;">
    </div>  
</div>



<div class="Services" id="target_service"> 
   
<div class="Serv-item">
    <h2>Services</h2>
     <p>
         We are offering you a Quality of Services by providing Material resources and courses related front-end technologies like HTML, CSS and JavaSCript.
         which help the beginner, who want to start their career towards development side.
         along with the content we also providing practing test aside which will be help to check their knowledge as well.
     </p>
 </div>
</div>

<div class="contact" id="target_contact">
    <h2 style="color: rgb(203, 203, 52);">Contact us</h2>
    <h3>The Learning Hub</h3>
    <h3>Hyderabad</h3>
    <div class="contact-details">
        <a href="mailto:gandhamraviteja2001@gmail.com?subject=Hello&body=How%20are%20you?" target="_blank">
            <img src="mail.png" alt="Email Icon">
            <span>gandhamraviteja2001@gmail.com</span>
        </a>
    </div>
    <div class="contact-details">
        <a href="https://www.linkedin.com/in/gandham-raviteja-8415031bb" target="_blank">
            <img src="linkedin-icon.png" alt="LinkedIn Icon">
            <span>LinkedIn</span>
        </a>
    </div>
    <div class="contact-details">
        <a href="#">
            <img src="phone-icon.png" alt="Phone Icon">
            <span>91+ 6302232951</span> 
        </a>
    </div>
</div>

<script src="navbar.js"></script>

</body>
</html>

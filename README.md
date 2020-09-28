<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}
body {font-family: "Lato", sans-serif;}

.tab {
  float: left;
  border: 1px solid #ccc;
  background-color: #f1f1f1;
  width: 30%;
  height: 300px;
}

.tab button {
  display: block;
  background-color: inherit;
  color: black;
  padding: 22px 16px;
  width: 100%;
  border: none;
  outline: none;
  text-align: left;
  cursor: pointer;
  transition: 0.3s;
  font-size: 17px;
}

.tab button:hover {
  background-color: #ddd;
}

.tab button.active {
  background-color: #ccc;
}

.tabcontent {
  float: left;
  padding: 0px 12px;
  border: none;
  width: 70%;
  border-left: none;
  height: 300px;
}
body{background-color:#566D7E;
}

.social-footer {
position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  padding: 1rem;
  background: #8a8a8a;
  display: -webkit-flex;
  display: -ms-flexbox;
  display: flex;
  -webkit-align-items: center;
      -ms-flex-align: center;
          align-items: center;
  -webkit-justify-content: space-between;
      -ms-flex-pack: justify;
          justify-content: space-between;
}

.social-footer .social-footer-icons li:last-of-type {
  margin-center:0;
}

.social-footer .social-footer-icons .fa {
  font-size: 1.3rem;
  color: #fefefe;
}

.social-footer .social-footer-icons .fa:hover {
  color: #4a4a4a;
  transition: color 0.3s ease-in;
}
.topnav input[type=text] {
  float: right;
  padding: 6px;
  border: none;
  margin-top: 8px;
  margin-right: 16px;
  font-size: 17px;
}
.topnav input[type=text] {
    border: 1px solid #ccc;
  }

</style>
</head>
<body>

<div class="tab">
  <button class="tablinks" onclick="openContent(event, 'Home')" id="defaultOpen">Home</button>
  <button class="tablinks" onclick="openContent(event, 'About')">About</button>
  <button class="tablinks" onclick="openContent(event, 'Services')">Services</button>
  <button class="tablinks" onclick="openContent(event, 'Contact us')">Contact us</button>
</div>
<div class="topnav"><img src="logo-black.png"> <input type="text" placeholder="Search..."></div>
<div id="Home" class="tabcontent">
  <h3>Home</h3>
  <p> We are Redefining Information Security.<br>We put systems in place to detect and prevent cybercrime, always keeping in mind the context 
  in which fraudulent transactions are concluded</p>
</div>

<div id="About" class="tabcontent">
  <h3>About us </h3>
  <p> We are a Company of Certified Ethical Hackers, Digital Forensics Practitioners that plans to empower
   Young Geeks.<br> We are a company that works with Mail&Gurdian Women into changing South Africa.
   we are here to inspire women to follow the technology carrer.
  M&G 200 Young SAns.Cybersec helps power the modern connected world with security made for people.<br>
  We protect digital content, applications, and devices with intuitive, people-centered and frictionless security. <br>
  Leading brands turn to Cybersec to secure everything from premium movies and live streaming sports, to sensitive financial and healthcare data, to mission-critical mobile applications. 
  We enable the trusted connections our customers depend on to deliver compelling content and experiences to millions of consumers around the world. 
  Cybersec helps partners to get to market faster, scale easily, protect valuable revenue streams, 
  and win new business.</p> 
</div>

<div id="Services" class="tabcontent">
  <h3>Services </h3>
  <p> We offer different services such as <ul><li>Information Security</li>
												<li>Information Technology</li>
												<li>WIFI installations</li>
												<li>Biometrics installations & Backup security storage</li>
												<li>Desktop and Helpdesk security systems</li>
												<li> Cyber security</li></ul></p>
												<img src="logo.jpg">
</div>

<div id="Contact us" class="tabcontent">
  <h3>Contact us</h3>
<p>We Can be contacted at 012 980 0000 and on different social platforms
    <ul class="menu simple">
<a href="https://www.facebook.com/"><i class="fa fa-facebook" aria-hidden="true"></i></a>
      <a href="https://www.instagram.com/?hl=en"><i class="fa fa-instagram" aria-hidden="true"></i></a>
      <a href="https://www.pinterest.com/"><i class="fa fa-pinterest-p" aria-hidden="true"></i></a>
      <a href="https://twitter.com/?lang=en"><i class="fa fa-twitter" aria-hidden="true"></i></a>
  </ul>
    </p>
</div>
<footer class="social-footer">
  <div class="social-footer-left">
    <a href="#"><img class="logo" src="logo-white.png"></a>Cybersec 2020 @Copyrights     You can follow us on our social media platforms
  </div>
  <div class="social-footer-icons">
  
    <ul class="menu simple">
      <a href="https://www.facebook.com/"><i class="fa fa-facebook" aria-hidden="true"></i></a>
      <a href="https://www.instagram.com/?hl=en"><i class="fa fa-instagram" aria-hidden="true"></i></a>
      <a href="https://www.pinterest.com/"><i class="fa fa-pinterest-p" aria-hidden="true"></i></a>
      <a href="https://twitter.com/?lang=en"><i class="fa fa-twitter" aria-hidden="true"></i></a>
    </ul>
  </div>
</footer>


<script>
function openContent(evt, Content) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(Content).style.display = "block";
  evt.currentTarget.className += " active";
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>
   
</body>
</html> 

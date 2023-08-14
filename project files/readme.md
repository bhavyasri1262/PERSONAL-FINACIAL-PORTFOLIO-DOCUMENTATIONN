<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Documentation</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
<body>
    <div id="header">
       <div class="container">
        <nav>
            <img src="images/logo.jpg" class="logo">
            <ul id="sidemenu">
                <li><a href="#header">Home</a></li><br>
                <li><a href="#about">About</a></li><br>
                <li><a href="#contact">Contact</a></li>
                <i class="fa fa-times" onclick="closemenu()"></i>
            </ul>
            <i class="fa fa-bars" onclick="openmenu()"></i>
        </nav>
        <div class="header-text">
            <p>Student</p>
            <h1>Hi, I'm <span>Lahari</span><br>From Vivekananda Degree College</h1>
        </div>
       </div> 
    </div>
    <!---about-->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="images/about.jpg">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>I am a dedicated,organised,methodical individual. I have good interpersonal skills, am an excellent team worker and 
                        keen and very willing to learn and develop new skills. I am reliable and dependable and often seek new 
                        responsibilities with in a wide range of employement areas.
                    </p>
                    <div class="tab-titles">
                    <p class="tab-links active-link" onclick="opentab('Skills')">Skills</p>
                    <p class="tab-links" onclick="opentab('Education')">Education</p>
                   </div>
                <div class="tab-contents active-tab" id="Skills">
                    <ul>
                        <li><span>Front-end Developer</span><br>HTML,CSS,JS</li><br>
                        <li><span>Salesforce</span><br>Administrator</li>
                    </ul>
                </div>
                <div class="tab-contents" id="Education">
                    <ul>
                        <li><span>2023</span><br>B.Sc Computer Science at Sri Vivekananda Degree College</li><br>
                        <li><span>2020</span><br>Intermediate-Dr.Himasekhar Junior College</li>
                        <li><span>2018</span><br>SSC at D.A.V Public School</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
    </div>
    <!----contact---->
<div id="contact">
    <div class="container">
       <div class="row">
            <div class="contact-left">
                 <h1 class="sub-title">Contact Me</h1><br>
                 <p><i class="fa fa-paper-plane-o"></i>contact@example.com</p><br>
                 <p><i class="fa fa-phone"></i>0987654321</p><br>
                 <div class="social-icons">
                    <a href="https://facebook.com/" class="fa fa-facebook"></a>
                    <a href="" class="fa fa-twitter"></a>
                    <a href="" class="fa fa-whatsapp"></a>
                    <a href="" class="fa fa-instagram"></a>
                    <a href="" class="fa fa-linkedin"></a>
                    </div><br>
                    <a href="images/lahari1_resume.pdf" download>
                        <button class="button">Resume</button>
                      </a> 
            </div>
            <div class="contact-right">
               <form>
                 <input type="text" name="Name" placeholder="Your Name"><br><br>
                 <input type="email" name="Email" placeholder="Your Email"><br><br>
                 <textarea name="Message" rows="6" placeholder="Your Message"></textarea><br><br>
                 <button type="submit" class="button">Submit</button>
               </form>
            </div>
       </div>
       <div class="copyright">
         <p>Copyright @Lahari.Portfolio Documentation</p>
       </div>
  </div>
   </div>
    <script>
        var tablinks=document.getElementsByClassName("tab-links");
        var tabcontents=document.getElementsByClassName("tab-contents");

        function opentab(tabname){
            for(tablink of tablinks){
                tablink.classList.remove("active-link");
             }
             for(tabcontent of tabcontents){
                tabcontent.classList.remove("active-tab");
             }
             event.currentTarget.classList.add("active-link");
             document.getElementById(tabname).classList.add("active-tab");
        }
    </script>
    <script>
        var sidemenu=document.getElementById("sidemenu");
        function openmenu(){
            sidemenu.style.right="0";
        }
        function closemenu(){
            sidemenu.style.right="-200px";
        }
    </script>
</body>
</html>

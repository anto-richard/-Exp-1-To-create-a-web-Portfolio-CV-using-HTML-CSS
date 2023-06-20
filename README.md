# Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS...

## AIM:

To write html & css code to create web portfolio/cv.

## ALGORITHM:

### STEP 1:

Create a html code for the portfolio.

### STEP 2:

Make style for the portfolio using css.

### STEP 3:

Link the css with html by link tag.

### STEP 4:

Verify the output by running the portfolio in any web browser.

## PROGRAM:

```html

Home Page HTML:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio Website</title>
    <link rel="stylesheet" href="pf.css">
</head>
<body>
    <div class="port">
        <nav>
            <img src="logo.png" class="logo">
            <ul>
                <li><a href="#">HOME</a></li>
                <li><a href="about me.html" target="_blank">ABOUT ME</a></li>
                <li><a href="cv.html" target="_blank">MY CV</a></li>
                <li><a href="myport.html" target="blank">MY PORTFOLIO</a></li>
                <li><a href="services.html" target="blank">SERVICES</a></li>
                <li><a href="hire me.html" target="blank">HIRE ME</a></li>
            </ul>
        </nav>
        <div class="name">
            <h1>I'm Anto <span> Richard</span></h1>
            <p>This is my official Portfolio website to showcase my all works related to <br> web development using html and css. </p>
            <a href="cv.html" target="_blank">Download My CV</a>
        </div>
        <div class="images">
            <img src="shape.jpg" class="shape">
            <img src="me.jpg" class="me">
        </div>

        <div class="social">
           <a href="#"><i class="fab fa-dribbble"></i></a>
           <a href="#"><i class="fab fa-instagram"></i></a>
           <a href="#"><i class="fab fa-behance"></i></a>
        </div>
    </div>

</body>
</html>

```

```css

HOME PAGE CSS:

*{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}

.port {
    position: relative;
    width: 100%;
    height: 100vh;
    background: url("bac.jpg") no-repeat center center fixed;
    background-size: cover;
    position: relative;
}

nav{
    display: flex;
    width: 84%;
    margin: auto;
    padding: 20px 0;
    align-items: center;
    justify-content: space-between;
}

.logo{
    width: 100px;
    cursor: pointer;
}

nav ul li {
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a{
    text-decoration: none;
    color: #000;
    font-weight: bold;
}

nav ul li a:hover{
    color: red;
}

.name{
    margin-left: 8%;
    margin-top: 15%;
}

.name h1{
    font-size: 50px;
    color: #212121;
    margin-bottom: 20px;
}

span{
    color: purple;
    
}

.name p{
    color: #555;
    line-height: 22px;
}

.name a{
    background: #212121;
    padding: 10px 18px;
    text-decoration: none;
    font-weight: bold;
    color: #fff;
    display: inline-block;
    margin: 30px 0;
    border-radius: 5px;
}

.images{
    width: 45%;
    height: 80%;
    position: absolute;
    bottom: 0;
    right: 100px;
}

.images img {
    height: 100%;
    position: absolute;
    left: 50%;
    bottom: 0;
    transform: translateX(-50%);
    transition: bottom 1s, left 1s;
}

.images:hover img {
    bottom: 50px;
    left: 50%;
}

.images:hover.shape{
    bottom: 40px;
}

.images:hover.me{
    left: 45%;
}

.social{
    margin-left: 8%;
    margin-top: 100px;
}

.social a{
    font-size: 30px;
    color: #212121;
    margin-right: 20px;
}

.social a:hover{
    color: orange;
}

#profile-pic {
    display: block;
    margin: 0 auto;
}

@media only screen and (max-width: 768px) {
    .port {
        overflow-x: hidden;
    }
    
    nav ul {
        display: none;
        width: 100%;
        background-color: #eff4fd;
        position: absolute;
        top: 70px;
        left: 0;
        padding: 10px 0;
        text-align: center;
        z-index: 1;
    }
    
    nav ul li {
        display: block;
        margin: 10px 0;
    }
    
    .logo{
        margin-left: 8%;
    }
    
    .name{
        margin-left: 8%;
        margin-top: 10%;
    }
    
    .name h1{
        font-size: 40px;
    }
    
    .name p{
        max-width: 100%;
        margin-bottom: 20px;
    }
    
    .images{
        position: static;
        margin-top: 20px;
        margin-bottom: 20px;
        width: 100%;
    }
    
    .social{
        margin-left: 8%;
        margin-top: 20px;
    }
}

```

```html

ABOUT ME HTML:

<!DOCTYPE html>
<html>
  <head>
    <title>About Me</title>
    <link rel="stylesheet" href="about me.css">
  </head>
  <body>
    <h2>About Me</h2>
    <p>Hi, my name is Anto Richard and I'm a web developer and also an expert in the domain of Artificial Intelligence & also in Machine Learning algorithms.
      <br> I have been working in this field for 4 years and have experience in HTML, CSS, C, Python and JavaScript.</p>
      <br>
    <p>In my free time, I enjoy playing cricket, solving Rubik's cube and photography. I also love to travel and explore new places.</p>
  </body>
</html>


```

```css

ABOUT ME CSS:

/* Set default font styles */
body {
    font-family: Arial, sans-serif;
    font-size: 16px;
    line-height: 1.5;
    color: #333;
  }
  
  /* Center header content */
  .header {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
  }
  
  /* Center the profile picture */
  #profile-pic {
    display: block;
    margin: 0 auto;
    width: 200px; /* adjust this to the appropriate size */
    border-radius: 50%;
  }
  
  #profile-pic:hover {
    opacity: 0.8;
  }
  
  
  /* Add some spacing between the profile picture and the contact info */
  .contact-info {
    margin-top: 20px;
  }
  
  /* Adjust the layout of the contact info */
  .contact-info h1 {
    margin: 0;
    font-size: 24px;
  }
  
  .contact-info p {
    margin: 0;
    font-size: 16px;
    line-height: 1.5;
  }
  
  /* Set styles for headings */
  h1, h2, h3 {
    font-weight: bold;
    margin-bottom: 10px;
  }
  
  h1 {
    font-size: 36px;
  }
  
  h2 {
    font-size: 24px;
  }
  
  h3 {
    font-size: 20px;
  }
  
  /* Set styles for paragraphs */
  p {
    margin-bottom: 10px;
  }
  
  /* Set styles for links */
  a {
    color: #007bff;
    text-decoration: none;
  }
  
  a:hover {
    text-decoration: underline;
  }
  
  /* Set styles for unordered lists */
  ul {
    margin-left: 20px;
    margin-bottom: 10px;
  }
  
  /* Style download link */
  .download-cv {
    text-align: center;
    margin: 20px 0;
  }
  
  .download-cv a {
    display: inline-block;
    padding: 10px 20px;
    background-color: #007bff;
    color: #fff;
    border-radius: 5px;
    text-decoration: none;
  }
  
  .download-cv a:hover {
    background-color: #0062cc;
  }

```

```html

CV HTML:

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CV - Anto Richard</title>
  <link rel="stylesheet" href="cv.css">
</head>
<body>
  <div class="header">
    <img src="me.jpg" alt="Profile Picture" id="profile-pic">
  </div>
    <div class="contact-info">
      <h1>Anto Richard</h1>
      <p>123 Main Street</p>
      <p>Canada, Montreal City, USA-H4X</p>
      <p>418-555-0101</p>
      <p>anto.richard@outlook.com</p>
    </div>
    
  <div class="summary">
    <h2>Professional Summary</h2>
    <p>A motivated and detail-oriented professional with over 2 years of experience in web development and in AI algorithms.<br>
       Skilled in HTML, CSS, JavaScript, and various web frameworks. Passionate about designing responsive and user-friendly websites.<br></p>
  </div>
    
  <div class="education">
    <h2>Education</h2>
    <div class="degree">
      <h3>Bachelor of Technology in Artificial Intelligence & Machine Learning</h3>
      <p>Saveetha Nagar, Chennai - 602105 Tamil Nadu, India</p>
      <p>Graduated November-2025</p>
    </div>
    <div class="certification">
      <h3>Machine Learning and Articulated Robot Workshop Certification</h3>
      <p>Issued by Madras Institute of Technology,MIT Rd, Radha Nagar, Chromepet, Chennai, Tamil Nadu 600044, May 2022</p>
    </div>
  </div>

  <!-- <div class="experience">
    <h2>Work Experience</h2>
    <div class="job">
      <h3>Web Developer</h3>
      <p>ABC Company, Canada, Montreal City, USA-H4X</p>
      <p>January 2027 - Present</p>
      <ul>
        <li>Designed and developed responsive and user-friendly websites for various clients</li>
        <li>Collaborated with cross-functional teams to deliver high-quality web solutions</li>
        <li>Implemented and maintained various web frameworks and tools to improve workflow efficiency</li>
      </ul>
    </div>
    <div class="job">
      <h3>Web Development Intern</h3>
      <p>PRECISE3DM - Reverse Engineering | 3D Scanning service | 3D Printing Service, <br> 
        Rajas Tower, No:2/461, 2nd Floor, Medavakkam Main Rd, Kovilambakkam, Chennai, Tamil Nadu 600129</p>
      <p>February 2023 - April 2023</p>
      <ul>
        <li>Assisted in the development and testing of various web projects</li>
        <li>Learned and applied various web frameworks and tools</li>
        <li>Participated in cross-functional team meetings and discussions</li>
      </ul>
    </div>
  </div>

  <div class="skills">
    <h2>Skills & Abilities</h2>
    <ul>
      <li>HTML</li>
      <li>CSS</li>
      <li>Machine Learning</li>
      <li>Artificial Intelligence</li>
      <li>JavaScript</li>
      <li>React</li>
      <li>Bootstrap</li>
      <li>Node.js</li>
      <li>Git</li>
      <li>Project Management</li>
      <li>Teamwork</li>
      <li>Communication</li>
    </ul>
  </div>

    <div class="download-cv">
        <a href="cv.pdf" download>Download My CV</a>
    </div> -->

    <div class="experience">
      <h2>Work Experience</h2>
      <div class="job">
        <h3>Web Developer</h3>
        <p>ABC Company, Canada, Montreal City, USA-H4X</p>
        <p>January 2027 - Present</p>
        <ul>
          <li>Designed and developed responsive and user-friendly websites for various clients</li>
          <li>Collaborated with cross-functional teams to deliver high-quality web solutions</li>
          <li>Implemented and maintained various web frameworks and tools to improve workflow efficiency</li>
        </ul>
      </div>
      <div class="job">
        <h3>Web Development Intern</h3>
        <p>PRECISE3DM - Reverse Engineering | 3D Scanning service | 3D Printing Service, <br> 
          Rajas Tower, No:2/461, 2nd Floor, Medavakkam Main Rd, Kovilambakkam, Chennai, Tamil Nadu 600129</p>
        <p>February 2023 - April 2023</p>
        <ul>
          <li>Assisted in the development and testing of various web projects</li>
          <li>Learned and applied various web frameworks and tools</li>
          <li>Participated in cross-functional team meetings and discussions</li>
        </ul>
      </div>
    </div>

```

```css

CV CSS:

/* Set default font styles */
body {
  font-family: Arial, sans-serif;
  font-size: 16px;
  line-height: 1.5;
  color: #333;
}

/* Center header content */
.header {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

/* Center the profile picture */
#profile-pic {
  display: block;
  margin: 0 auto;
  width: 200px; /* adjust this to the appropriate size */
  border-radius: 50%;
}

#profile-pic:hover {
  opacity: 0.8;
}


/* Add some spacing between the profile picture and the contact info */
.contact-info {
  margin-top: 20px;
}

/* Adjust the layout of the contact info */
.contact-info h1 {
  margin: 0;
  font-size: 24px;
}

.contact-info p {
  margin: 0;
  font-size: 16px;
  line-height: 1.5;
}

/* Set styles for headings */
h1, h2, h3 {
  font-weight: bold;
  margin-bottom: 10px;
}

h1 {
  font-size: 36px;
}

h2 {
  font-size: 24px;
}

h3 {
  font-size: 20px;
}

/* Set styles for paragraphs */
p {
  margin-bottom: 10px;
}

/* Set styles for links */
a {
  color: #007bff;
  text-decoration: none;
}

a:hover {
  text-decoration: underline;
}

/* Set styles for unordered lists */
ul {
  margin-left: 20px;
  margin-bottom: 10px;
}

/* Style download link */
.download-cv {
  text-align: center;
  margin: 20px 0;
}

.download-cv a {
  display: inline-block;
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  border-radius: 5px;
  text-decoration: none;
}

.download-cv a:hover {
  background-color: #0062cc;
}


.experience {
  display: flex;
  flex-direction: column;
}

.job {
  border: 1px solid #ccc;
  padding: 20px;
  margin-bottom: 20px;
}

.job h3 {
  margin-top: 0;
}

.job p {
  margin: 10px 0;
}

.job ul {
  margin: 0;
  padding: 0;
  list-style: none;
}

.job ul li {
  margin-bottom: 10px;
}

@media only screen and (min-width: 768px) {
  .experience {
    flex-direction: row;
    justify-content: space-between;
  }
  
  .job {
    width: 48%;
  }
}

```

```html

HIRE ME HTML:

<!DOCTYPE html>
<html>
  <head>
    <title>Hire Me</title>
    <link rel="stylesheet" type="text/css" href="hire me.css">
  </head>
  <body>
    <div class="container">
      <h1>Hire Me</h1>
      <p>Hi there! I'm excited to hear that you're interested in hiring me. <br>
        Please fill out the form below with your details and I'll get back to you as soon as possible.</p>
      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>

        <label for="phone">Phone:</label>
        <input type="tel" id="phone" name="phone" required>

        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="5" required></textarea>

        <button type="submit">Send</button>
      </form>
    </div>
  </body>
</html>

```

```css

HIRE ME CSS:

.container {
    max-width: 600px;
    margin: 0 auto;
    padding: 40px;
    background-color: #f7f7f7;
    border-radius: 5px;
  }
  
  h1 {
    text-align: center;
  }
  
  form {
    display: flex;
    flex-direction: column;
  }
  
  label {
    margin-bottom: 10px;
  }
  
  input[type="text"],
  input[type="email"],
  input[type="tel"],
  textarea {
    margin-bottom: 20px;
    padding: 10px;
    border: none;
    border-radius: 5px;
  }
  
  button {
    background-color: #0077cc;
    color: #fff;
    padding: 10px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  button:hover {
    background-color: #005da6;
  }

```

```html

SERVICES HTML:

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Services Page</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <header>
      <nav>
        <ul>
            <link rel="stylesheet" type="text/css" href="services.css">
        </ul>
      </nav>
    </header>
    
    <main>
        <section class="services">
            <div class="container">
              <div class="service">
                <h2>Web Design</h2>
                <p>We create visually appealing website designs that capture the essence of your brand and engage your audience. Our designs are tailored to your unique requirements, ensuring that your website stands out from the competition.</p>
              </div>
              <div class="service">
                <h2>Web Development</h2>
                <p>We develop custom websites that are fast, secure, and optimized for search engines. Our team of developers can handle all aspects of the development process, from front-end design to back-end coding and database integration.</p>
                <a href="#">Learn More</a>
              </div>
              <div class="service">
                <h2>SEO Optimization</h2>
                <p>We offer search engine optimization services to help your website rank higher in search engine results pages (SERPs). Our team of SEO experts can help you identify keywords and phrases that your target audience is searching for and optimize your website accordingly.</p>
                <a href="#">Learn More</a>
              </div>
            </div>
          </section>          
    </main>
    
    <footer>
        <center>
      <p>&copy; 2023 Services Page. All rights reserved.</p>
    </center>
    </footer>
  </body>
</html>

```

```css

SERVICES CSS:

/* Basic Styles for the Services Page */

/* Global Styles */
body {
    font-family: Arial, Helvetica, sans-serif;
    margin: 0;
    padding: 0;
  }
  
  /* Header Styles */
  header {
    background-color: #333;
    color: #fff;
    display: flex;
    justify-content: center;
    padding: 10px;
  }
  
  nav {
    max-width: 960px;
    width: 100%;
  }
  
  nav ul {
    display: flex;
    justify-content: space-between;
    list-style-type: none;
    margin: 0;
    padding: 0;
  }
  
  nav ul li a {
    color: #fff;
    font-size: 18px;
    text-decoration: none;
    transition: color 0.3s ease;
  }
  
  nav ul li a:hover {
    color: #c7c7c7;
  }
  
  nav ul li a.active {
    color: #c7c7c7;
  }
  
  /* Services Styles */
  .services {
    background-color: #f2f2f2;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 0 auto;
    max-width: 960px;
    padding: 40px 0;
  }
  
  .services h1 {
    text-align: center;
    margin-bottom: 40px;
  }
  
  .service {
    background-color: #fff;
    border: 1px solid #d7d7d7;
    border-radius: 4px;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    margin-bottom: 20px;
    padding: 20px;
    text-align: center;
  }
  .service h2 {
    font-size: 24px;
    margin-bottom: 10px;
  }
  .service p {
    font-size: 16px;
    line-height: 24px;
  }
  .service a {
    display: inline-block;
    margin-top: 10px;
    padding: 10px 20px;
    background-color: #2ecc71;
    color: #fff;
    border-radius: 4px;
    text-decoration: none;
    transition: background-color 0.2s ease;
  }
  .service a:hover {
    background-color: #27ae60;
  }

```

## OUTPUT:

![p1](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/103d75ca-86ba-4904-b274-ebea7a49ff1e)

![p2](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/b14a6cf1-22cf-4848-9b1a-23dde23542ce)

![p3](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/b83fd129-2184-4ae5-9a8b-ebb71b10df07)

![p4](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/7e6b1e91-ad4e-4bd7-b8ef-f8e3f66ffccd)

![p5](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/9bbd74fe-de43-4801-aae0-67a12a5200e5)

![p6](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/5cfe7ae6-d8df-45db-90d0-de009aed82e4)

![p7](https://github.com/anto-richard/-Exp-1-To-create-a-web-Portfolio-CV-using-HTML-CSS/assets/93427534/c200847c-22fa-4feb-b2de-f5206ff03d6c)

## RESULT:

Thus by using the html & css code to create web portfolio/cv has been created and output has been verified.


**** Portfolio-website-for-prolync


###Folder structure 

portfolio-website/
 ├─ index.html
 ├─ style.css
 ├─ script.js
 ├─ README.md
 └─ assets/
     └─ (put your images/resume here)



####### My Portfolio Website

A simple portfolio website built using **HTML**, **CSS**, and **JavaScript**.  
You can use this as a starting point and add your own projects and details.  

##  Technologies Used
- HTML5
- CSS3
- JavaScript
- (Optional) React for advanced features

## Structure
- `index.html` – Main page structure
- `style.css` – Stylesheet
- `script.js` – JavaScript for interactivity
- `assets/` – Images, resume, icons


---

######### index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Your Name | Portfolio</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <h1>Your Name</h1>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="hero">
    <h2>Hello, I'm <span>Your Name</span></h2>
    <p>Aspiring Web Developer | React Enthusiast</p>
    <a href="#projects" class="btn">View My Work</a>
  </section>

  <section id="about">
    <h2>About Me</h2>
    <p>Write a short bio about your skills, education, and interests here.</p>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="project-grid">
      <div class="project-card">
        <h3>Project 1</h3>
        <p>Short description of your project.</p>
        <a href="#">View Project</a>
      </div>
      <div class="project-card">
        <h3>Project 2</h3>
        <p>Short description of your project.</p>
        <a href="#">View Project</a>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <form>
      <input type="text" placeholder="Name" required />
      <input type="email" placeholder="Email" required />
      <textarea placeholder="Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Your Name. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>


#####Stye.csss

  
  * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}
body {
  line-height: 1.6;
  background: #f4f4f4;
  color: #333;
}
header {
  background: #222;
  color: #fff;
  padding: 20px 0;
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  margin: auto;
}
nav ul {
  display: flex;
  list-style: none;
}
nav ul li {
  margin-left: 20px;
}
nav ul li a {
  color: #fff;
  text-decoration: none;
}
#hero {
  text-align: center;
  padding: 80px 20px;
  background: #007bff;
  color: #fff;
}
.btn {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 20px;
  background: #fff;
  color: #007bff;
  text-decoration: none;
  border-radius: 5px;
}
section {
  padding: 60px 20px;
  width: 80%;
  margin: auto;
}
.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
}
.project-card {
  background: #fff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
form {
  display: flex;
  flex-direction: column;
}
form input, form textarea, form button {
  margin-bottom: 15px;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}
footer {
  text-align: center;
  padding: 20px;
  background: #222;
  color: #fff;
}


script.js

// Smooth scrolling for nav links
document.querySelectorAll('nav a').forEach(link => {
  link.addEventListener('click', e => {
    e.preventDefault();
    document.querySelector(link.getAttribute('href'))
      .scrollIntoView({ behavior: 'smooth' });
  });
});




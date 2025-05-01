# Ex01 Portfolio

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
### HTML:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Your Portfolio</title>
  <link rel="stylesheet" href="Jeffport.css" />
</head>
<body>
  <header class="fade-in-top">
    <div class="container">
      <h1>Jeffy Brailin</h1>
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <section class="hero fade-in">
        <div class="container">
          <img src="profile.jpg" alt="Your Photo" class="profile-img" />
          <h2>Hello, I'm a Developer & Student</h2>
          <p>I love building beautiful websites and learning new technologies.</p>
          <a href="#contact" class="btn">Get in Touch</a>
        </div>
      </section>
      
    </div>
  </section>

  <section id="about" class="section fade-in-delay">
    <div class="container">
      <h2>About Me</h2>
      <p>I'm a Second year Computer Science student passionate about web development, UI/UX design, and building impactful digital experiences.</p>
    </div>
  </section>

  <section id="projects" class="section fade-in-delay">
    <div class="container">
      <h2>Projects</h2>
      <div class="grid">
        <div class="card glow">
          <h3>Project 1</h3>
          <p>Artificial Intelligence Chatbot</p>
        </div>
        <div class="card glow">
          <h3>Project 2</h3>
          <p>Fake News Detection Website</p>
        </div>
      </div>
    </div>
  </section>

  <section id="skills" class="section fade-in-delay">
    <div class="container">
      <h2>Skills</h2>
      <ul class="skills">
        <li class="glow">HTML</li>
        <li class="glow">CSS</li>
        <li class="glow">JavaScript</li>
        <li class="glow">Git</li>
        <li class="glow">UI/UX Design</li>
      </ul>
    </div>
  </section>

  <section id="contact" class="section contact fade-in-delay">
    <div class="container">
      <h2>Contact Me</h2>
      <p>Email: jeffybrailin@gmail.com</p>
      <p>LinkedIn: linkedin.com/in/jeffybrailin</p>
    </div>
  </section>

  <footer class="fade-in-bottom">
    <div class="container">
      <p>© 2025 Your Name. All rights reserved.</p>
    </div>
  </footer>
</body>
</html>

```
### CSS:
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
  }
  
  body {
    font-family: 'Segoe UI', sans-serif;
    background: #f9f9f9;
    color: #333;
    line-height: 1.6;
    overflow-x: hidden;
  }
  
  .container {
    width: 90%;
    max-width: 1100px;
    margin: auto;
    padding: 20px 0;
  }
  
  header {
    background: #1f1f1f;
    color: white;
    padding: 20px 0;
    position: sticky;
    top: 0;
    z-index: 10;
  }
  
  header h1 {
    float: left;
    margin-left: 10px;
  }
  
  nav {
    float: right;
  }
  
  nav a {
    color: white;
    text-decoration: none;
    margin: 0 15px;
    font-weight: 500;
    transition: color 0.3s ease;
  }
  
  nav a:hover {
    color: #ff7272;
  }
  
  .hero {
    background: linear-gradient(to right, #ff5f6d, #ffc371);
    color: white;
    text-align: center;
    padding: 100px 20px;
  }
  
  .hero h2 {
    font-size: 2.5rem;
    margin-bottom: 15px;
  }
  
  .hero .btn {
    display: inline-block;
    margin-top: 20px;
    padding: 12px 30px;
    background: white;
    color: #ff5f6d;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
    transition: transform 0.2s ease;
  }
  
  .hero .btn:hover {
    transform: scale(1.05);
  }
  
  .section {
    padding: 60px 0;
    background: white;
  }
  
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
  }
  
  .card {
    background: #f1f1f1;
    padding: 20px;
    border-radius: 10px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  }
  
  .skills {
    display: flex;
    flex-wrap: wrap;
    list-style: none;
    gap: 15px;
  }
  
  .skills li {
    background: #eee;
    padding: 10px 20px;
    border-radius: 20px;
    font-weight: bold;
    transition: background 0.3s ease;
  }
  
  .skills li:hover {
    background: #ff7272;
    color: white;
  }
  
  .contact {
    background: #ffe1e1;
    text-align: center;
  }
  
  footer {
    text-align: center;
    padding: 20px 0;
    background: #1f1f1f;
    color: white;
  }
  
  /* Animations */
  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  @keyframes fadeInTop {
    from {
      opacity: 0;
      transform: translateY(-30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  @keyframes fadeInBottom {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  .fade-in {
    animation: fadeIn 1s ease forwards;
  }
  
  .fade-in-delay {
    opacity: 0;
    animation: fadeIn 1.5s ease forwards;
  }
  
  .fade-in-top {
    animation: fadeInTop 1s ease forwards;
  }
  
  .fade-in-bottom {
    animation: fadeInBottom 1.2s ease forwards;
  }
  
  /* Glow Effect */
  .glow {
    transition: box-shadow 0.3s ease;
  }
  
  .glow:hover {
    box-shadow: 0 0 15px rgba(255, 94, 98, 0.6);
  }
  
  .profile-img {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    object-fit: cover;
    border: 5px solid white;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
    margin-bottom: 20px;
    transition: transform 0.3s ease;
  }
  
  .profile-img:hover {
    transform: scale(1.05);
  }
  
```

## OUTPUT
![image](https://github.com/user-attachments/assets/d90855de-f50b-4e76-8ad5-1cab20c37530)


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.

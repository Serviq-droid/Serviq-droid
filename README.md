<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Andre Cortez Gamboa | Portfolio</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;600&display=swap');

  * {
    margin: 0; padding: 0; box-sizing: border-box;
  }

  body {
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
    color: #f0f0f0;
    overflow-x: hidden;
  }

  header {
    padding: 2rem 1rem;
    text-align: center;
    position: relative;
    z-index: 10;
  }

  header h1 {
    font-weight: 600;
    font-size: 3rem;
    background: linear-gradient(90deg, #00d2ff, #3a47d5);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: gradientMove 5s ease infinite;
  }

  @keyframes gradientMove {
    0% {background-position: 0%;}
    50% {background-position: 100%;}
    100% {background-position: 0%;}
  }

  header p {
    margin-top: 0.5rem;
    font-size: 1.3rem;
    color: #a0a0a0;
  }

  nav {
    margin-top: 1.5rem;
    display: flex;
    justify-content: center;
    gap: 2rem;
  }

  nav a {
    text-decoration: none;
    color: #7fd1ff;
    font-weight: 600;
    transition: color 0.3s ease;
  }

  nav a:hover {
    color: #00d2ff;
  }

  main {
    max-width: 900px;
    margin: 3rem auto;
    padding: 0 1rem;
  }

  section {
    margin-bottom: 4rem;
  }

  h2 {
    font-size: 2rem;
    border-bottom: 3px solid #00d2ff;
    padding-bottom: 0.3rem;
    margin-bottom: 1rem;
  }

  p, li {
    font-weight: 300;
    line-height: 1.6;
    color: #d0d7de;
  }

  ul {
    list-style: none;
    margin-top: 0.8rem;
  }

  ul li::before {
    content: "🔥";
    margin-right: 0.5rem;
  }

  .projects {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
    gap: 2rem;
  }

  .project-card {
    background: rgba(255, 255, 255, 0.05);
    border-radius: 15px;
    padding: 1.5rem;
    box-shadow: 0 8px 24px rgb(0 210 255 / 0.3);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 15px 40px rgb(0 210 255 / 0.6);
  }

  .project-card h3 {
    color: #00d2ff;
    margin-bottom: 0.7rem;
  }

  .project-card a {
    color: #7fd1ff;
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
  }

  .project-card a:hover {
    color: #00d2ff;
    text-decoration: underline;
  }

  footer {
    text-align: center;
    padding: 2rem 1rem;
    background: #0a1a2b;
    color: #4a90e2;
  }

  .btn-contact {
    display: inline-block;
    padding: 0.8rem 1.8rem;
    border-radius: 30px;
    background: #00d2ff;
    color: #0a1a2b;
    font-weight: 700;
    text-decoration: none;
    margin-top: 1rem;
    transition: background 0.3s ease;
  }

  .btn-contact:hover {
    background: #3a47d5;
    color: #fff;
  }

  /* Floating animation for emoji */
  @keyframes float {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-15px); }
  }

  .wave {
    display: inline-block;
    animation: float 3s ease-in-out infinite;
    font-size: 2rem;
  }
</style>
</head>
<body>

<header>
  <h1>Andre Cortez Gamboa <span class="wave">👋</span></h1>
  <p>Junior Software Developer | Systems Engineer</p>
  <nav>
    <a href="#about">About Me</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<main>
  <section id="about">
    <h2>About Me</h2>
    <p>Hi! I’m Andre, a passionate junior software developer and systems engineer. I love transforming ideas into efficient code and learning cutting-edge technologies.</p>
  </section>

  <section id="skills">
    <h2>Skills & Tools</h2>
    <ul>
      <li>JavaScript (ES6+), Java, HTML5, CSS3</li>
      <li>React (in progress), Node.js, Express</li>
      <li>Databases: MySQL, PostgreSQL</li>
      <li>Version Control: Git, GitHub</li>
      <li>VS Code, Terminal, DevOps basics</li>
    </ul>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="projects">
      <div class="project-card">
        <h3>Portfolio Website</h3>
        <p>A modern, responsive portfolio built with HTML, CSS, and JavaScript.</p>
        <a href="https://github.com/Serviq-droid/portfolio" target="_blank">View on GitHub →</a>
      </div>
      <div class="project-card">
        <h3>Java Blog Platform</h3>
        <p>Simple blog engine developed in Java with MySQL database integration.</p>
        <a href="https://github.com/Serviq-droid/blog-java" target="_blank">View on GitHub →</a>
      </div>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <p>If you want to collaborate or just say hi, send me a message!</p>
    <a class="btn-contact" href="mailto:andrecortez889@gmail.com">📧 Email Me</a>
  </section>
</main>

<footer>
  <p>© 2025 Andre Cortez Gamboa. All rights reserved.</p>
</footer>

</body>
</html>

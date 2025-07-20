# vaidooriya-portfolio
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Vaidooriya's Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    body {
      background: linear-gradient(135deg, #2b005c, #0b022d, #000924);
      color: #ffffff;
      overflow-x: hidden;
      position: relative;
    }

    header {
      text-align: center;
      padding: 4rem 2rem 2rem;
      background: rgba(0, 0, 0, 0.5);
      backdrop-filter: blur(10px);
      position: relative;
      z-index: 2;
    }

    h1 {
      font-size: 3rem;
      text-shadow: 2px 2px 10px #9a00ff;
      color: #ffcbff;
    }

    .intro {
      font-size: 1.3rem;
      margin-top: 1rem;
      color: #e4d4ff;
    }

    .section {
      width: 420px;
      height: 420px;
      margin: 6rem auto;
      background: rgba(0, 0, 0, 0.6);
      padding: 2rem;
      border-radius: 50%;
      box-shadow: 0 0 40px rgba(128, 0, 255, 0.6);
      backdrop-filter: blur(8px);
      text-align: center;
      overflow: hidden;
      display: flex;
      flex-direction: column;
      justify-content: center;
      position: relative;
      opacity: 0;
      transform: translateX(100px);
      transition: all 1s ease-in-out;
      animation: float 5s infinite alternate ease-in-out, dance 3s infinite;
      z-index: 2;
    }

    .section.visible {
      opacity: 1;
      transform: translateX(0);
    }

    .section.left {
      transform: translateX(-100px);
    }

    h2 {
      color: #ff92ff;
      margin-bottom: 0.8rem;
      font-size: 1.7rem;
      text-shadow: 1px 1px 5px #000;
    }

    p, ul {
      font-size: 1rem;
      line-height: 1.5;
    }

    ul {
      padding-left: 1.2rem;
    }

    ul li {
      margin-bottom: 0.4rem;
    }

    footer {
      text-align: center;
      padding: 2rem;
      background: rgba(0, 0, 0, 0.5);
      font-size: 0.95rem;
      color: #ccc;
    }

    a {
      color: #ffea67;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    @keyframes float {
      0% { transform: translateY(0); }
      100% { transform: translateY(-12px); }
    }

    @keyframes dance {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.05); }
    }

    .side-pattern {
      position: fixed;
      top: 0;
      bottom: 0;
      width: 80px;
      background: repeating-linear-gradient(45deg, #3c006e, #3c006e 10px, #220034 10px, #220034 20px);
      z-index: 1;
    }

    .left-pattern {
      left: 0;
    }

    .right-pattern {
      right: 0;
    }

    .butterfly {
      position: absolute;
      width: 150px;
      z-index: 0;
      opacity: 0.4;
      animation: fly 60s infinite linear;
      pointer-events: none;
    }

    @keyframes fly {
      0% { transform: translateX(-200px) translateY(0) scale(1); }
      25% { transform: translateX(25vw) translateY(-20vh) rotate(90deg) scale(1.2); }
      50% { transform: translateX(50vw) translateY(30vh) rotate(180deg) scale(1); }
      75% { transform: translateX(75vw) translateY(-10vh) rotate(270deg) scale(1.1); }
      100% { transform: translateX(100vw) translateY(0) rotate(360deg) scale(1); }
    }

    .star {
      position: absolute;
      width: 40px;
      height: 40px;
      background: white;
      border-radius: 50%;
      opacity: 0.8;
      animation: fall linear infinite;
    }

    @keyframes fall {
      0% {
        transform: translateY(0);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh);
        opacity: 0;
      }
    }
  </style>
</head>

<body>
  <div class="side-pattern left-pattern"></div>
  <div class="side-pattern right-pattern"></div>

  <!-- Floating Butterflies -->
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Butterfly_icon_2.svg/2048px-Butterfly_icon_2.svg.png" class="butterfly" style="top:10%; left:-150px;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Butterfly_icon_2.svg/2048px-Butterfly_icon_2.svg.png" class="butterfly" style="top:60%; left:-200px; animation-delay: 10s;">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Butterfly_icon_2.svg/2048px-Butterfly_icon_2.svg.png" class="butterfly" style="top:40%; left:-250px; animation-delay: 20s;">

  <header>
    <h1>Vaidooriya V</h1>
    <p class="intro">Aspiring Full-Stack Developer | Java Enthusiast | Creative Web Designer</p>
  </header>

  <section class="section left">
    <h2>About Me</h2>
    <p>Hello! I'm Vaidooriya from Tamil Nadu — a tech enthusiast who builds interactive, animated, and responsive websites. I specialize in Java, HTML, and CSS and thrive in creating projects that combine logic and design. I’m fluent in Tamil, English, Malayalam, and basic Kannada, and bring strong soft skills like communication, problem-solving, and adaptability.</p>
  </section>

  <section class="section">
    <h2>Projects</h2>
    <ul>
      <li>Personal Portfolio Website</li>
      <li>Landing Page UI Design</li>
      <li>Falling Stars Animation Project</li>
    </ul>
  </section>

  <section class="section left">
    <h2>Certifications</h2>
    <ul>
      <li>Java Programming Certification</li>
      <li>HTML & CSS Certification</li>
      <li>English Proficiency</li>
      <li>PPT Presentation Skills</li>
      <li>Science Project Presentation</li>
    </ul>
  </section>

  <section class="section">
    <h2>Skills</h2>
    <ul>
      <li>Effective Communication</li>
      <li>Problem Solving</li>
      <li>Teamwork</li>
      <li>Adaptability</li>
    </ul>
  </section>

  <section class="section left">
    <h2>Languages</h2>
    <ul>
      <li>Tamil</li>
      <li>English</li>
      <li>Malayalam</li>
      <li>Basic Kannada</li>
    </ul>
  </section>

  <section class="section">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:vaidooriya80@gmail.com">vaidooriya80@gmail.com</a></p>
    <p>LinkedIn: <a href="https://www.linkedin.com/in/vaidooriya-vijayasekar" target="_blank">vaidooriya-vijayasekar</a></p>
  </section>

  <footer>
    <p>&copy; 2025 Vaidooriya V. Designed with ✨ by Me.</p>
  </footer>

  <script>
    // Scroll animation
    const sections = document.querySelectorAll('.section');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.2 });
    sections.forEach(sec => observer.observe(sec));

    // Falling stars
    for (let i = 0; i < 50; i++) {
      const star = document.createElement('div');
      star.className = 'star';
      star.style.left = `${Math.random() * 100}vw`;
      star.style.top = `${Math.random() * -100}vh`;
      star.style.animationDuration = `${3 + Math.random() * 5}s`;
      document.body.appendChild(star);
    }
  </script>
</body>
</html>

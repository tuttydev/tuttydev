<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My GitHub Profile</title>
  <style>
    :root {
      --primary-color: #4a90e2;
      --secondary-color: #f0f4f8;
      --accent-color: #d9edf7;
      --text-color: #333;
    }

    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--secondary-color);
      color: var(--text-color);
    }

    header {
      background: var(--primary-color);
      color: white;
      padding: 15px;
      text-align: center;
    }

    .typewriter h1, .typewriter h2 {
      display: inline-block;
      overflow: hidden;
      white-space: nowrap;
      border-right: 3px solid white; /* Adjust for cursor effect */
      animation: typing 3s steps(40, end), blink-caret .75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink-caret {
      from, to { border-color: transparent; }
      50% { border-color: white; }
    }

    .container {
      max-width: 800px;
      margin: 20px auto;
      padding: 20px;
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      animation: fadeInUp 1s ease-in-out;
    }

    h3 {
      cursor: pointer;
      color: var(--primary-color);
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 0;
      border-bottom: 1px solid var(--accent-color);
    }

    h3:hover {
      color: darken(var(--primary-color), 10%);
    }

    .content {
      display: none;
      padding: 10px 0;
      border-bottom: 1px solid var(--accent-color);
      overflow: hidden;
      transition: max-height 0.5s ease;
    }

    .content.show {
      display: block;
      animation: fadeInUp 0.5s ease forwards;
    }

    ul {
      list-style-type: none;
      padding-left: 0;
    }

    li {
      margin: 5px 0;
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 0.5s ease forwards;
    }

    .content.show li {
      animation: fadeInUp 0.5s ease forwards;
      animation-delay: 0.1s;
    }

    a {
      color: var(--primary-color);
      text-decoration: none;
      transition: text-decoration 0.3s ease, color 0.3s ease;
    }

    a:hover {
      text-decoration: underline;
      color: darken(var(--primary-color), 10%);
    }

    footer {
      text-align: center;
      padding: 20px;
      font-size: 0.9em;
    }

    @keyframes fadeInUp {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const toggles = document.querySelectorAll('.container h3');
      toggles.forEach(toggle => {
        toggle.addEventListener('click', () => {
          const content = toggle.nextElementSibling;
          if (content.style.display === 'none' || content.style.display === '') {
            content.style.display = 'block';
            content.classList.add('show');
            content.style.maxHeight = content.scrollHeight + 'px';
          } else {
            content.style.display = 'none';
            content.classList.remove('show');
            content.style.maxHeight = '0';
          }
          toggle.querySelector('span').textContent = toggle.querySelector('span').textContent === '+' ? '−' : '+';
        });
      });
    });
  </script>
</head>
<body>
<header class="typewriter">
  <h1>Welcome to My GitHub Profile! 👋</h1>
  <h2>About Me</h2>
</header>
<div class="container">
  <p>Hello! I'm Alasi Olatunde, a passionate software developer with a keen interest in creating dynamic and user-friendly applications. My journey in the tech world is fueled by a love for problem-solving and a constant drive to learn and grow. I specialize in web, mobile and desktop app development, with a strong focus on backend and frontend technologies.</p>

  <h3>Skills and Technologies <span>+</span></h3>
  <div class="content">
    <ul>
      <li><strong>Frontend Development:</strong> HTML, CSS, JavaScript, React, Vue.js</li>
      <li><strong>Backend Development:</strong> Python, Django, Flask, Node.js, Express</li>
      <li><strong>Database Management:</strong> MySQL, PostgreSQL</li>
      <li><strong>UI/UX Design:</strong> Figma</li>
      <li><strong>Mobile Development:</strong> Kivy, Flutter</li>
      <li><strong>Other Technologies:</strong> Git, Docker, AWS</li>
    </ul>
  </div>

  <h3>Projects <span>+</span></h3>
  <div class="content">
    <ul>
      <li><strong>Project 1:</strong> <a href="https://github.com/tuttydev/ecommerce-website">Comprehensive Ecommerce Website</a></li>
      <li><strong>Project 2:</strong> <a href="https://github.com/tuttydev/hospital-management-system">Hospital Management System</a></li>
      <li><strong>Project 3:</strong> <a href="https://github.com/tuttydev/hair-salon-website">Hair Salon Website</a></li>
      <li><strong>Project 4:</strong> <a href="https://github.com/tuttydev/biology-quiz-app">Biology Quiz App</a></li>
      <li><strong>Project 5:</strong> <a href="https://github.com/tuttydev/sales-app">Sales App</a></li>
    </ul>
  </div>

  <h3>Get In Touch <span>+</span></h3>
  <div class="content">
    <p>You can reach me at: <a href="mailto:alasiolatunde@gmail.com">alasiolatunde@gmail.com</a></p>
    whatsapp : +2348137335772
  </div>
</div>
<footer>
  <p>© 2023 Alasi Olatunde. All Rights Reserved.</p>
</footer>
</body>
</html>

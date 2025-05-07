!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tenzin Norphel | Portfolio</title>
  <style>
    body {
      font-family: Georgia, serif;
      margin: 0;
      background: url('background.jpg') no-repeat center center fixed;
      background-size: cover;
      color: #fff;
    }
    nav {
      background: rgba(0, 0, 0, 0.7);
      padding: 1em;
      text-align: center;
    }
    nav a {
      color: #fff;
      margin: 0 1em;
      text-decoration: none;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .tab {
      display: none;
      padding: 2em;
      background: rgba(0, 0, 0, 0.6);
    }
    .tab.active {
      display: block;
    }
    footer {
      text-align: center;
      padding: 1em;
      font-size: 0.9em;
      background: rgba(0, 0, 0, 0.7);
      color: #ccc;
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" onclick="showTab('about')">About</a>
    <a href="#" onclick="showTab('skills')">Skills</a>
    <a href="#" onclick="showTab('achievements')">Achievements</a>
    <a href="#" onclick="showTab('education')">Education</a>
    <a href="#" onclick="showTab('expertise')">Field Expertise</a>
  </nav>

  <div id="about" class="tab active">
    <h2>About Me</h2>
    <p>I'm Tenzin Norphel, an EECS student at UC Berkeley with strong interests in robotics, control systems, AI, and microfabrication.</p>
  </div>

  <div id="skills" class="tab">
    <h2>Skills</h2>
    <ul>
      <li>Python, MATLAB, C++, Java, Git</li>
      <li>ROS, MuJoCo, Sentaurus, EasyEXPERT</li>
      <li>Control Theory, Computer Vision, AI/ML</li>
    </ul>
  </div>

  <div id="achievements" class="tab">
    <h2>Achievements</h2>
    <ul>
      <li>NASA MCA Project Intern</li>
      <li>Built full RISC-V CPU in Logisim</li>
      <li>Led visual servoing and grasp control for Sawyer+Allegro Hand</li>
    </ul>
  </div>

  <div id="education" class="tab">
    <h2>Education</h2>
    <p><strong>University of California, Berkeley</strong><br>BS in Electrical Engineering and Computer Science<br>Expected Graduation: Dec 2025</p>
  </div>

  <div id="expertise" class="tab">
    <h2>Field Expertise</h2>
    <ul>
      <li>Robotics Systems and Path Planning</li>
      <li>Control System Design and State Estimation</li>
      <li>Microfabrication Process Flow and Semiconductor Device Simulation</li>
    </ul>
  </div>

  <footer>
    &copy; 2025 Tenzin Norphel — Portfolio powered by GitHub Pages
  </footer>

  <script>
    function showTab(tabId) {
      document.querySelectorAll('.tab').forEach(tab => {
        tab.classList.remove('active');
      });
      document.getElementById(tabId).classList.add('active');
    }
  </script>
</body>
</html>

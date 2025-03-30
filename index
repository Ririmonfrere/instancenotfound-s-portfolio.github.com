<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>InstanceNotFound | Scripter</title>
  <style>
    /* Global Styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Arial', sans-serif;
      background-color: #000;
      color: #fff;
      line-height: 1.6;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
      scroll-behavior: smooth;
    }

    h1, h2, h3 {
      font-family: 'Roboto', sans-serif;
      margin-bottom: 20px;
    }

    a {
      text-decoration: none;
    }

    /* Sidebar */
    .sidebar {
      position: fixed;
      top: 0;
      left: 0;
      height: 100%;
      width: 250px;
      background-color: #222;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding-top: 50px;
      z-index: 100;
      padding-left: 20px;
      padding-right: 20px;
    }

    .sidebar a {
      color: white;
      padding: 20px;
      font-size: 1.2rem;
      border-radius: 8px;
      margin-bottom: 15px;
      text-align: center;
      transition: background-color 0.3s ease;
      width: 100%;
      text-align: left;
    }

    .sidebar a:hover {
      background-color: #4CAF50;
    }

    .sidebar a:first-child {
      margin-top: 0;
    }

    /* Navbar */
    nav {
      display: flex;
      justify-content: space-between;
      padding: 20px;
      background-color: #111;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 100;
    }

    nav ul {
      display: flex;
      gap: 30px;
    }

    nav a {
      color: #fff;
      font-size: 1.1rem;
      padding: 5px 10px;
      transition: all 0.3s ease;
    }

    nav a:hover {
      background-color: #4CAF50;
      border-radius: 5px;
    }

    /* Hero Section */
    .hero {
      text-align: center;
      margin-top: 100px;
      padding: 60px 0;
    }

    .hero h1 {
      font-size: 3.5rem;
      margin-bottom: 10px;
    }

    .hero p {
      font-size: 1.4rem;
      margin-bottom: 40px;
      color: #bbb;
    }

    .hero a {
      padding: 12px 20px;
      background-color: #4CAF50;
      color: white;
      font-size: 1.2rem;
      border-radius: 8px;
      transition: background-color 0.3s ease;
    }

    .hero a:hover {
      background-color: #45a049;
    }

    /* Projects Section */
    .projects {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      margin-top: 80px;
      padding: 50px 0;
      width: 100%;
    }

    .project {
      background-color: #222;
      width: 70%;
      max-width: 900px;
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.7);
      margin-bottom: 40px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      margin-left: auto;
      margin-right: auto;
    }

    .project:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.9);
    }

    .project h3 {
      font-size: 2rem;
      margin-bottom: 10px;
    }

    .project p {
      color: #bbb;
    }

    /* Can Do / Can't Do Cards */
    .cards-section {
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 50px 0;
      margin-top: 50px;
    }

    .card {
      background-color: #333;
      width: 300px;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.7);
      opacity: 0;
      transform: translateY(50px);
      transition: opacity 0.5s ease-out, transform 0.5s ease-out;
      margin-bottom: 30px;
    }

    .card.visible {
      opacity: 1;
      transform: translateY(0);
    }

    .card h3 {
      font-size: 1.6rem;
      margin-bottom: 10px;
    }

    .card ul {
      list-style: none;
    }

    .card li {
      margin-bottom: 10px;
      color: #bbb;
    }

    /* Contact Section */
    .contact {
      text-align: center;
      padding: 60px 0;
      background-color: #111;
    }

    .contact h2 {
      font-size: 2.5rem;
      margin-bottom: 30px;
    }

    .contact a {
      padding: 12px 20px;
      background-color: #4CAF50;
      color: white;
      font-size: 1.1rem;
      border-radius: 8px;
      transition: background-color 0.3s ease;
    }

    .contact a:hover {
      background-color: #45a049;
    }

    /* Form Styling */
    .contact-form {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      gap: 20px;
      max-width: 500px;
      margin: 0 auto;
      background-color: #222;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.7);
    }

    .contact-form input, .contact-form textarea {
      width: 100%;
      padding: 12px;
      border-radius: 8px;
      border: none;
      font-size: 1rem;
    }

    .contact-form button {
      padding: 12px 20px;
      background-color: #4CAF50;
      color: white;
      font-size: 1.2rem;
      border-radius: 8px;
      border: none;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    .contact-form button:hover {
      background-color: #45a049;
    }

  </style>
</head>
<body>
  <nav>
    <div class="logo">InstanceNotFound</div>
    <ul>
      <li><a href="#hero">Homepage</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Sidebar Navigation -->
  <div class="sidebar">
    <a href="#hero">Homepage</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
    <a href="https://discord.com/users/InstanceNotFound">Discord</a>
    <a href="https://www.youtube.com/@instancenotfound">YouTube</a>
  </div>

  <!-- Hero Section -->
  <div class="hero" id="hero">
    <h1>Hello! I’m InstanceNotFound</h1>
    <p>Scripter | Belgium</p>
    <a href="#projects">View My Work</a>
  </div>

  <!-- Projects Section -->
  <div class="projects" id="projects">
    <div class="project">
      <h3>Sans Multiverse</h3>
      <p>A game inspired by *UnderTale*, where players fight powerful bosses, gain experience, and challenge even more dangerous Sans characters.</p>
    </div>
    <div class="project">
      <h3>Superpower Battleground</h3>
      <p>An action-packed game where players harness the abilities of various anime characters, facing off in intense battles to become the ultimate fighter.</p>
    </div>
    <div class="project">
      <h3>Soul Unleashed</h3>
      <p>A role-playing game where you begin as a beginner and fight to gain experience and power, ultimately striving to become a legendary Soul Reaper.</p>
    </div>
  </div>

  <!-- Can Do / Can't Do Section -->
  <div class="cards-section">
    <div class="card" id="can-do">
      <h3>Can Do</h3>
      <ul>
        <li>Chest Opening System</li>
        <li>Gamepass & Dev Product Systems</li>
        <li>Memory Management</li>
        <li>Matchmaking System</li>
        <li>VIP Access & Perks</li>
        <li>Chat Filtering & Moderation</li>
        <li>Custom Animations</li>
        <li>Teleportation System</li>
        <li>Sprinting & Stamina System (without stamina)</li>
      </ul>
    </div>
    <div class="card" id="cant-do">
      <h3>Can't Do</h3>
      <ul>
        <li>Data Store (Not Experienced)</li>
        <li>Complex AI Systems</li>
        <li>Advanced Physics Systems</li>
      </ul>
    </div>
  </div>

  <!-- Contact Section -->
  <div class="contact" id="contact">
    <h2>Contact Me</h2>
    <p>If you'd like to collaborate or have any questions, feel free to reach out!</p>

    <!-- Contact Form -->
    <form class="contact-form" id="contactForm">
      <input type="text" id="discordUsername" placeholder="Your Discord Username" required>
      <textarea id="message" rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </div>

  <script>
    // Reveal "Can Do" and "Can't Do" cards with animation
    window.addEventListener('load', function () {
      const canDoCard = document.getElementById('can-do');
      const cantDoCard = document.getElementById('cant-do');
      setTimeout(function () {
        canDoCard.classList.add('visible');
        cantDoCard.classList.add('visible');
      }, 500); // Slight delay for a smooth transition
    });

    document.getElementById('contactForm').addEventListener('submit', function(event) {
      event.preventDefault();

      const discordUsername = document.getElementById('discordUsername').value;
      const message = document.getElementById('message').value;

      const payload = {
        content: `**Message from:** ${discordUsername}\n**Message:** ${message}`
      };

      fetch('https://discord.com/api/webhooks/1355684398346801243/W97_mK6urDOQYdvIaUKOcLgeLjEUMhsR84QmCtoHbzzHwFuBf77Db1oZ2CWsZyD4LMmOY', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify(payload),
      })
      .then(response => response.json())
      .then(data => {
        alert('Message Sent!');
        document.getElementById('contactForm').reset();
      })
      .catch(error => {
        alert('Error sending message.');
      });
    });
  </script>
</body>
</html>

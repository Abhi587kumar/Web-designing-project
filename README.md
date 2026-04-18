<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Student Web Designing Project</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #f4f4f4;
    }
    header {
      background: #333; color: #fff;
      padding: 20px; text-align: center;
    }
    nav ul {
      list-style: none; margin: 0; padding: 0;
      display: flex; justify-content: center;
      background: #444;
    }
    nav ul li {
      margin: 0 15px;
    }
    nav ul li a {
      color: #fff; text-decoration: none;
      padding: 10px;
    }
    nav ul li a:hover {
      background: #666; border-radius: 5px;
    }
    .container {
      padding: 20px;
    }
    .card {
      background: #fff; padding: 20px;
      margin: 20px 0; border-radius: 8px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }
    footer {
      background: #333; color: #fff;
      text-align: center; padding: 15px;
      position: fixed; bottom: 0; width: 100%;
    }
    button {
      background: #007BFF; color: #fff;
      border: none; padding: 10px 15px;
      border-radius: 5px; cursor: pointer;
    }
    button:hover {
      background: #0056b3;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to My Web Designing Project</h1>
    <p>Learning HTML, CSS, and JavaScript</p>
  </header>

  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#gallery">Gallery</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <div class="container">
    <section id="home" class="card">
      <h2>Home</h2>
      <p>This project demonstrates the implementation of a simple responsive website using core web technologies.</p>
    </section>

    <section id="about" class="card">
      <h2>About</h2>
      <p>Web designing combines creativity and coding to build functional, user‑friendly, and visually appealing websites.</p>
    </section>

    <section id="gallery" class="card">
      <h2>Gallery</h2>
      <img src="https://via.placeholder.com/300" alt="Sample Image">
      <img src="https://via.placeholder.com/300" alt="Sample Image">
    </section>

    <section id="contact" class="card">
      <h2>Contact</h2>
      <form id="contactForm">
        <label>Name:</label><br>
        <input type="text" id="name" required><br><br>
        <label>Email:</label><br>
        <input type="email" id="email" required><br><br>
        <button type="submit">Submit</button>
      </form>
      <p id="message"></p>
    </section>
  </div>

  <footer>
    <p>&copy; 2026 Web Designing Project | Created by Avinash Sharma</p>
  </footer>

  <script>
    // Simple form validation and interaction
    document.getElementById("contactForm").addEventListener("submit", function(e) {
      e.preventDefault();
      const name = document.getElementById("name").value;
      const email = document.getElementById("email").value;
      document.getElementById("message").innerText =
        "Thank you, " + name + "! We will contact you at " + email + ".";
    });
  </script>
</body>
</html>

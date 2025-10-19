<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Sameer Ahmad - Portfolio</title>

  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;700&family=Poppins:wght@300;400;500;700&display=swap" rel="stylesheet">

  <style>
    * {
      scroll-behavior: smooth;
      box-sizing: border-box;
    }

    body {
      background-color: #0a0a0a;
      color: #eaeaea;
      font-family: 'Poppins', sans-serif;
      overflow-x: hidden;
    }

    /* Navbar */
    .navbar {
      background: rgba(15, 15, 15, 0.9);
      border-bottom: 2px solid #0ff;
      backdrop-filter: blur(12px);
    }

    .navbar-brand {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.5rem;
      color: #00ffff !important;
      text-shadow: 0 0 12px #00ffff;
    }

    .nav-link {
      color: #fff !important;
      transition: 0.3s;
    }

    .nav-link:hover {
      color: #00ffff !important;
      text-shadow: 0 0 10px #00ffff;
    }

    /* Home Section */
    #home {
      background: radial-gradient(circle at top left, #001f3f, #000);
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;
      padding: 100px 20px 50px;
    }

    .profile-img {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      border: 3px solid #00ffff;
      box-shadow: 0 0 40px #00ffff;
      object-fit: cover;
      margin-bottom: 20px;
      transition: transform 0.4s ease;
    }

    .profile-img:hover {
      transform: rotate(5deg) scale(1.05);
    }

    h1 {
      font-family: 'Orbitron', sans-serif;
      color: #00ffff;
      text-shadow: 0 0 20px #00ffff;
    }

    h4, h5 {
      color: #ccc;
    }

    .description {
      max-width: 700px;
      color: #aaa;
      font-size: 1.1rem;
      margin-top: 15px;
    }

    /* Projects Section */
    #projects {
      background: linear-gradient(145deg, #141414, #1b1b1b);
      padding: 100px 0;
    }

    .section-title {
      font-family: 'Orbitron', sans-serif;
      color: #00ffff;
      text-align: center;
      margin-bottom: 60px;
      text-shadow: 0 0 20px #00ffff;
    }

    .project-card {
      background: #111;
      border: 1px solid #00ffff;
      border-radius: 15px;
      padding: 30px;
      color: #eaeaea;
      text-align: center;
      box-shadow: 0 0 15px rgba(0, 255, 255, 0.3);
      transition: 0.3s;
    }

    .project-card:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 25px rgba(0, 255, 255, 0.7);
    }

    .project-card h3 {
      color: #00ffff;
      font-family: 'Orbitron', sans-serif;
      margin-bottom: 15px;
    }

    /* Contact Section */
    #contact {
      background: radial-gradient(circle at bottom right, #001f3f, #000);
      padding: 100px 0;
      color: white;
    }

    .contact-card {
      background: rgba(15, 15, 15, 0.9);
      border: 1px solid #00ffff;
      box-shadow: 0 0 25px rgba(0, 255, 255, 0.3);
      border-radius: 20px;
      padding: 40px;
    }

    .form-control {
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid #00ffff;
      color: #fff;
    }

    .form-control::placeholder {
      color: #aaa;
    }

    .btn-neon {
      background: #00ffff;
      color: #000;
      font-weight: 600;
      border: none;
      border-radius: 8px;
      padding: 10px;
      width: 100%;
      transition: 0.3s ease;
      box-shadow: 0 0 15px #00ffff;
    }

    .btn-neon:hover {
      background: #0ff;
      box-shadow: 0 0 25px #00ffff;
      transform: scale(1.05);
    }

    /* Footer */
    footer {
      background: #000;
      color: #999;
      text-align: center;
      padding: 20px;
      border-top: 1px solid #00ffff;
      box-shadow: 0 -2px 20px rgba(0, 255, 255, 0.2);
    }

    /* Animation */
    [data-animate] {
      opacity: 0;
      transform: translateY(40px);
      transition: all 0.8s ease;
    }

    [data-animate].visible {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#home">Sameer Ahmad</a>
      <div>
        <a class="nav-link" href="#projects">Projects</a>
        <a class="nav-link" href="#contact">Contact</a>
      </div>
    </div>
  </nav>

  <!-- Home -->
  <section id="home">
    <img src="sameer.jpg" alt="Profile Picture" class="profile-img">
    <h1>Sameer Ahmad</h1>
    <h4>Registration No: FA23-BCS-130</h4>
    <h5>Comsats University Islamabad</h5>
    <p class="description">
      A tech enthusiast passionate about AI, Flutter, and full-stack development — building innovative digital experiences that merge creativity with logic.
    </p>
  </section>

  <!-- Projects -->
  <section id="projects">
    <div class="container">
      <h2 class="section-title">Featured Projects</h2>
      <div class="row g-4">

        <div class="col-md-6 col-lg-4" data-animate>
          <div class="project-card">
            <h3>Smart Attendance System</h3>
            <p>An AI-powered facial recognition attendance system built using Python and OpenCV for real-time verification and record automation.</p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4" data-animate>
          <div class="project-card">
            <h3>Flutter Expense Tracker</h3>
            <p>A mobile app developed in Flutter to track expenses, visualize spending trends with graphs, and manage budgets intelligently.</p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4" data-animate>
          <div class="project-card">
            <h3>AI Resume Analyzer</h3>
            <p>A web-based tool using Natural Language Processing (NLP) to evaluate resumes and provide hiring recommendations to recruiters.</p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4" data-animate>
          <div class="project-card">
            <h3>Weather Predictor Dashboard</h3>
            <p>A Python-based dashboard using machine learning to predict local weather patterns with visualization using Matplotlib.</p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4" data-animate>
          <div class="project-card">
            <h3>Smart Campus Navigation</h3>
            <p>A Flutter + Firebase mobile app that helps new students navigate the university campus using Google Maps API integration.</p>
          </div>
        </div>

        <div class="col-md-6 col-lg-4" data-animate>
          <div class="project-card">
            <h3>Personal Portfolio Website</h3>
            <p>This portfolio — built using HTML, CSS, and Bootstrap — showcasing creative UI, responsive design, and smooth animations.</p>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="container">
      <h2 class="section-title">Contact Me</h2>
      <div class="col-md-8 mx-auto contact-card" data-animate>
        <form>
          <div class="mb-3">
            <label class="form-label text-info">Full Name</label>
            <input type="text" class="form-control" placeholder="Enter your name">
          </div>
          <div class="mb-3">
            <label class="form-label text-info">Email</label>
            <input type="email" class="form-control" placeholder="Enter your email">
          </div>
          <div class="mb-3">
            <label class="form-label text-info">Message</label>
            <textarea class="form-control" rows="4" placeholder="Type your message"></textarea>
          </div>
          <button type="submit" class="btn-neon">Send Message</button>
        </form>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    © 2025 Sameer Ahmad | Comsats University Islamabad
  </footer>

  <script>
    // Scroll animations
    const items = document.querySelectorAll('[data-animate]');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        }
      });
    }, { threshold: 0.2 });
    items.forEach(item => observer.observe(item));
  </script>
</body>
</html>



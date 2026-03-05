<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Kanairo Haven Rising Foundation | Refuge, Hope & New Beginnings</title>
  <meta name="description" content="Supporting orphans, GBV survivors, and girls escaping FGM in Nairobi. Providing safety, education, healing, and a fresh start."/>
  
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet"/>
  
  <!-- Font Awesome for icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  
  <style>
    :root {
      --primary: #e74c3c;      /* Warm red - hope & urgency */
      --primary-dark: #c0392b;
      --secondary: #2c3e50;    /* Dark blue-gray - trust */
      --light: #f8f9fa;
      --success: #27ae60;
    }
    
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    
    body {
      font-family: 'Poppins', sans-serif;
      line-height: 1.7;
      color: #333;
      background: #fff;
    }
    
    .container {
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 20px;
    }
    
    header {
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 1000;
      background: rgba(44, 62, 80, 0.95);
      backdrop-filter: blur(8px);
      transition: background 0.3s;
    }
    
    header.scrolled {
      background: #2c3e50;
    }
    
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 0;
    }
    
    .logo {
      color: white;
      font-size: 1.6rem;
      font-weight: 700;
      text-decoration: none;
    }
    
    .logo span {
      color: var(--primary);
    }
    
    .nav-links {
      display: flex;
      list-style: none;
    }
    
    .nav-links li {
      margin-left: 35px;
    }
    
    .nav-links a {
      color: white;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s;
    }
    
    .nav-links a:hover {
      color: var(--primary);
    }
    
    /* Hero */
    #hero {
      height: 100vh;
      min-height: 700px;
      background: linear-gradient(rgba(0,0,0,0.65), rgba(0,0,0,0.65)), 
                  url('https://images.unsplash.com/photo-1522202176988-66273c2b033f?ixlib=rb-4.0.3&auto=format&fit=crop&w=1350&q=80') center/cover no-repeat;
      color: white;
      display: flex;
      align-items: center;
      text-align: center;
    }
    
    .hero-content {
      max-width: 800px;
      margin: 0 auto;
    }
    
    .hero h1 {
      font-size: 3.8rem;
      margin-bottom: 20px;
      line-height: 1.2;
    }
    
    .hero p {
      font-size: 1.3rem;
      margin-bottom: 35px;
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
    }
    
    .btn {
      display: inline-block;
      padding: 14px 36px;
      background: var(--primary);
      color: white;
      text-decoration: none;
      border-radius: 50px;
      font-weight: 600;
      transition: all 0.3s;
      margin: 10px;
    }
    
    .btn:hover {
      background: var(--primary-dark);
      transform: translateY(-3px);
      box-shadow: 0 10px 20px rgba(231,76,60,0.3);
    }
    
    .btn-outline {
      background: transparent;
      border: 2px solid white;
    }
    
    /* Sections */
    section {
      padding: 100px 0;
    }
    
    h2 {
      text-align: center;
      font-size: 2.6rem;
      margin-bottom: 20px;
      color: var(--secondary);
    }
    
    h2 span {
      color: var(--primary);
    }
    
    .about, .causes, .impact, .donate, .contact {
      background: var(--light);
    }
    
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 30px;
      margin-top: 60px;
    }
    
    .card {
      background: white;
      border-radius: 12px;
      overflow: hidden;
      box-shadow: 0 5px 15px rgba(0,0,0,0.08);
      transition: transform 0.3s;
    }
    
    .card:hover {
      transform: translateY(-10px);
    }
    
    .card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }
    
    .card-content {
      padding: 25px;
    }
    
    .card h3 {
      margin-bottom: 15px;
      color: var(--secondary);
    }
    
    /* Donate section */
    .donate {
      background: linear-gradient(135deg, #2c3e50, #34495e);
      color: white;
      text-align: center;
    }
    
    .donate .container {
      max-width: 700px;
    }
    
    .donate-form {
      margin: 50px 0;
      display: flex;
      flex-direction: column;
      gap: 20px;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }
    
    input, select, textarea {
      padding: 15px;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
    }
    
    footer {
      background: #1a252f;
      color: #aaa;
      text-align: center;
      padding: 60px 0 30px;
    }
    
    .social-icons a {
      color: white;
      font-size: 1.6rem;
      margin: 0 15px;
      transition: color 0.3s;
    }
    
    .social-icons a:hover {
      color: var(--primary);
    }
    
    @media (max-width: 768px) {
      .hero h1 { font-size: 2.8rem; }
      .nav-links { display: none; } /* Add hamburger menu JS later if needed */
    }
  </style>
</head>
<body>

  <header id="header">
    <div class="container">
      <nav>
        <a href="#" class="logo">Kanairo <span>Haven Rising</span> Foundation</a>
        <ul class="nav-links">
          <li><a href="#hero">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#causes">Our Work</a></li>
          <li><a href="#impact">Impact</a></li>
          <li><a href="#donate">Donate</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <section id="hero">
    <div class="hero-content">
      <h1>Refuge. Healing. A New Beginning in Kanairo</h1>
      <p>We provide safe shelter, counseling, education, and empowerment to poor orphans, survivors of gender-based violence, and girls who have escaped FGM — turning pain into hope and survival into thriving.</p>
      <a href="#donate" class="btn">Donate Now</a>
      <a href="#contact" class="btn btn-outline">Get Involved</a>
    </div>
  </section>

  <section id="about" class="about">
    <div class="container">
      <h2>Who We <span>Are</span></h2>
      <p style="text-align:center; max-width:800px; margin:0 auto 40px; font-size:1.2rem;">
        Kanairo Haven Rising Foundation is a Nairobi-based NGO dedicated to offering refuge and comprehensive support to the most vulnerable: orphans facing extreme poverty, women and girls surviving GBV, and those fleeing female genital mutilation. In the heart of Kanairo — a city of second chances — we help them rebuild lives with safety, dignity, education, skills training, and long-term empowerment.
      </p>
    </div>
  </section>

  <section id="causes" class="causes">
    <div class="container">
      <h2>Our Core <span>Causes</span></h2>
      <div class="grid">
        <div class="card">
          <img src="https://images.unsplash.com/photo-1503454537195-1dcabb9d2a69?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Orphans support">
          <div class="card-content">
            <h3>Orphan Care</h3>
            <p>Food, shelter, education, emotional support, and family-like environment for children who have lost everything.</p>
          </div>
        </div>
        <div class="card">
          <img src="https://images.unsplash.com/photo-1524178232363-1fb2b075b655?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="GBV survivors">
          <div class="card-content">
            <h3>GBV Recovery</h3>
            <p>Trauma counseling, legal aid, medical care, and safe housing for survivors of gender-based violence.</p>
          </div>
        </div>
        <div class="card">
          <img src="https://images.unsplash.com/photo-1519345182560-3f2917c472ef?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="FGM escapees">
          <div class="card-content">
            <h3>FGM Escape Support</h3>
            <p>Emergency refuge, protection, rehabilitation, education, and advocacy for girls who have run away from FGM.</p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section id="impact" class="impact">
    <div class="container">
      <h2>Impact & <span>Stories</span></h2>
      <p style="text-align:center; font-size:1.2rem; max-width:900px; margin:0 auto 50px;">
        Since our founding, we have sheltered over 180 individuals, provided counseling to 250+ survivors, supported education for 120 children, and helped many begin new, independent lives.
      </p>
      <!-- You can add real testimonials, counters, or photos here later -->
    </div>
  </section>

  <section id="donate" class="donate">
    <div class="container">
      <h2>Help Us <span>Change Lives</span></h2>
      <p>Your donation provides food, shelter, medical care, counseling, school fees, and vocational training — giving someone a real chance to rise.</p>
      
      <form class="donate-form" action="#" method="post">
        <input type="text" placeholder="Full Name" required/>
        <input type="email" placeholder="Email Address" required/>
        <select required>
          <option value="">Choose Donation Amount (KES)</option>
          <option value="500">KES 500 - Monthly Sponsor</option>
          <option value="2000">KES 2,000 - Emergency Support</option>
          <option value="5000">KES 5,000 - Education Fund</option>
          <option value="10000">KES 10,000 - Shelter & Food</option>
          <option value="other">Other Amount</option>
        </select>
        <textarea placeholder="Message / Dedication (optional)"></textarea>
        <button type="submit" class="btn" style="width:100%; font-size:1.3rem; padding:18px;">Donate Securely</button>
      </form>
      
      <p style="margin-top:30px; font-size:0.95rem;">We accept M-Pesa, PayPal, bank transfer. Contact us for details. Thank you for being the change.</p>
    </div>
  </section>

  <section id="contact" class="contact">
    <div class="container">
      <h2>Get in <span>Touch</span></h2>
      <p style="text-align:center; font-size:1.2rem;">
        Reach out to volunteer, partner, or learn more about how you can support our work in Kanairo.
      </p>
      <div style="text-align:center; margin:40px 0; font-size:1.1rem;">
        <p><i class="fas fa-phone"></i> +254 7XX XXX XXX</p>
        <p><i class="fas fa-envelope"></i> info@kanairohavenrising.org</p>
        <p><i class="fas fa-map-marker-alt"></i> Nairobi, Kenya</p>
      </div>
    </div>
  </section>

  <footer>
    <div class="container">
      <p>&copy; 2026 Kanairo Haven Rising Foundation. All rights reserved.</p>
      <div class="social-icons" style="margin:25px 0;">
        <a href="#"><i class="fab fa-facebook-f"></i></a>
        <a href="#"><i class="fab fa-twitter"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
        <a href="#"><i class="fab fa-linkedin-in"></i></a>
      </div>
      <p style="font-size:0.9rem; opacity:0.7;">Built with hope for a better tomorrow.</p>
    </div>
  </footer>

  <script>
    // Simple scroll effect for header
    window.addEventListener('scroll', () => {
      const header = document.getElementById('header');
      header.classList.toggle('scrolled', window.scrollY > 100);
    });
  </script>

</body>
</html>

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>KS DIGITAL SERVICES</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
/* Elegant Color Palette */
:root {
  --primary: #2c3e50;
  --secondary: #3498db;
  --accent: #e74c3c;
  --gold: #d4af37;
  --light: #f8f9fa;
  --dark: #1a1a2e;
  --gray: #6c757d;
  --radius: 12px;
  --shadow: 0 8px 30px rgba(0, 0, 0, 0.08);
  --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

/* Base Styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
  color: var(--dark);
  line-height: 1.6;
  min-height: 100vh;
  position: relative;
  overflow-x: hidden;
}

body::before {
  content: '';
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: 
    radial-gradient(circle at 20% 80%, rgba(52, 152, 219, 0.03) 0%, transparent 20%),
    radial-gradient(circle at 80% 20%, rgba(212, 175, 55, 0.03) 0%, transparent 20%);
  z-index: -1;
}

/* Header */
header {
  background: linear-gradient(135deg, var(--primary) 0%, #1a1a2e 100%);
  color: white;
  padding: 2.5rem 1rem;
  text-align: center;
  position: relative;
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
  border-bottom: 4px solid var(--gold);
}

.logo-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 0.5rem;
}

.logo-icon {
  width: 60px;
  height: 60px;
  background: var(--gold);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 0.5rem;
  box-shadow: 0 4px 12px rgba(212, 175, 55, 0.3);
}

.logo-icon i {
  font-size: 1.8rem;
  color: var(--primary);
}

h1 {
  font-family: 'Playfair Display', serif;
  font-size: 2.5rem;
  font-weight: 700;
  letter-spacing: 1px;
  margin-bottom: 0.5rem;
  position: relative;
  display: inline-block;
}

h1::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 3px;
  background: var(--gold);
  border-radius: 2px;
}

.tagline {
  font-size: 1.1rem;
  font-weight: 300;
  color: rgba(255, 255, 255, 0.85);
  max-width: 600px;
  margin: 0 auto;
  margin-top: 1rem;
}

/* Home Button */
.home-btn {
  position: absolute;
  top: 20px;
  left: 20px;
  background: rgba(255, 255, 255, 0.15);
  color: white;
  padding: 0.7rem 1.5rem;
  border-radius: 50px;
  text-decoration: none;
  font-weight: 500;
  font-size: 0.9rem;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.2);
  transition: var(--transition);
}

.home-btn:hover {
  background: rgba(255, 255, 255, 0.25);
  transform: translateY(-2px);
  box-shadow: 0 6px 15px rgba(0, 0, 0, 0.1);
}

/* Main Content */
main {
  max-width: 900px;
  margin: 3rem auto;
  padding: 0 1.5rem;
}

.content-wrapper {
  background: white;
  border-radius: var(--radius);
  box-shadow: var(--shadow);
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
}

.content-wrapper::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(90deg, var(--primary), var(--gold));
}

/* Services Section */
.services-intro {
  text-align: center;
  margin-bottom: 2.5rem;
}

.services-intro h2 {
  font-family: 'Playfair Display', serif;
  font-size: 1.8rem;
  color: var(--primary);
  margin-bottom: 0.8rem;
}

.services-intro p {
  color: var(--gray);
  max-width: 600px;
  margin: 0 auto;
}

/* Buttons Grid */
.buttons-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.action-btn {
  background: white;
  border: 1px solid #eaeaea;
  border-radius: var(--radius);
  padding: 1.5rem;
  text-decoration: none;
  color: var(--dark);
  display: flex;
  align-items: center;
  gap: 1.2rem;
  transition: var(--transition);
  position: relative;
  overflow: hidden;
}

.action-btn:hover {
  transform: translateY(-5px);
  box-shadow: 0 12px 25px rgba(0, 0, 0, 0.1);
  border-color: var(--secondary);
}

.action-btn::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 4px;
  height: 100%;
  background: var(--secondary);
  opacity: 0;
  transition: opacity 0.3s;
}

.action-btn:hover::before {
  opacity: 1;
}

.btn-icon {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.3rem;
  color: white;
  flex-shrink: 0;
}

.btn-content {
  flex-grow: 1;
}

.btn-content h3 {
  font-size: 1.1rem;
  margin-bottom: 0.3rem;
  color: var(--primary);
}

.btn-content p {
  font-size: 0.85rem;
  color: var(--gray);
  line-height: 1.4;
}

.arrow-icon {
  color: var(--gray);
  font-size: 1rem;
  transition: transform 0.3s;
}

.action-btn:hover .arrow-icon {
  transform: translateX(5px);
  color: var(--secondary);
}

/* Color variations for buttons */
.btn-call .btn-icon { background: var(--secondary); }
.btn-directions .btn-icon { background: #2ecc71; }
.btn-whatsapp .btn-icon { background: #25D366; }
.btn-instagram .btn-icon { background: #E1306C; }
.btn-youtube .btn-icon { background: #FF0000; }
.btn-printer .btn-icon { background: var(--gold); }

/* Contact Info */
.contact-info {
  margin-top: 3rem;
  padding-top: 2rem;
  border-top: 1px solid #eee;
  text-align: center;
}

.contact-info p {
  color: var(--gray);
  margin-bottom: 0.5rem;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
}

.phone-number {
  font-size: 1.3rem;
  color: var(--primary);
  font-weight: 600;
  margin-top: 0.5rem;
}

/* Footer */
footer {
  text-align: center;
  padding: 2rem 1rem;
  color: var(--gray);
  font-size: 0.9rem;
  background: var(--primary);
  color: rgba(255, 255, 255, 0.8);
  margin-top: 3rem;
}

.footer-content {
  max-width: 900px;
  margin: 0 auto;
}

.copyright {
  margin-top: 1rem;
  font-size: 0.8rem;
  color: rgba(255, 255, 255, 0.6);
}

/* Responsive Design */
@media (max-width: 768px) {
  h1 {
    font-size: 2rem;
  }
  
  .home-btn {
    position: relative;
    top: 0;
    left: 0;
    margin-bottom: 1.5rem;
    display: inline-flex;
  }
  
  .content-wrapper {
    padding: 1.8rem;
  }
  
  .buttons-grid {
    grid-template-columns: 1fr;
  }
  
  .logo-icon {
    width: 50px;
    height: 50px;
  }
}

@media (max-width: 480px) {
  h1 {
    font-size: 1.7rem;
  }
  
  .tagline {
    font-size: 1rem;
  }
  
  .action-btn {
    padding: 1.2rem;
  }
}

/* Animation for page load */
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

.content-wrapper, header {
  animation: fadeInUp 0.6s ease-out forwards;
}
</style>

</head>
<body>

<header>

   <h2>KS DIGITAL SERVICES</h2>
  <a class="home-btn" href="https://ksdigitalservice.pw/">
    <i class="fas fa-home"></i>
    Home Page
  </a>
</header>

<main>
  <div class="content-wrapper">
    <div class="services-intro">
      <h2>Connect With Us</h2>
      
    </div>
    
    <div class="buttons-grid">
      <!-- Call Button -->
      <a class="action-btn btn-call" href="tel:+917893845696">
        <div class="btn-icon">
          <i class="fas fa-phone-alt"></i>
        </div>
        <div class="btn-content">
          <h3>Call Now 7893845696</h3>
          
        </div>
        <div class="arrow-icon">
          <i class="fas fa-chevron-right"></i>
        </div>
      </a>
      
      <!-- Directions Button -->
      <a class="action-btn btn-directions" href="https://maps.app.goo.gl/VfZ4fHYw6nYFTavB6" target="_blank">
        <div class="btn-icon">
          <i class="fas fa-map-marker-alt"></i>
        </div>
        <div class="btn-content">
          <h3>Get Directions</h3>
        </div>
        <div class="arrow-icon">
          <i class="fas fa-chevron-right"></i>
        </div>
      </a>
      
      <!-- WhatsApp Button -->
      <a class="action-btn btn-whatsapp" href="https://wa.me/7893845696" target="_blank">
        <div class="btn-icon">
          <i class="fab fa-whatsapp"></i>
        </div>
        <div class="btn-content">
          <h3>WhatsApp</h3>
        </div>
        <div class="arrow-icon">
          <i class="fas fa-chevron-right"></i>
        </div>
      </a>
      
      <!-- Instagram Button -->
      <a class="action-btn btn-instagram" href="https://www.instagram.com/ksdigitalservice/" target="_blank">
        <div class="btn-icon">
          <i class="fab fa-instagram"></i>
        </div>
        <div class="btn-content">
          <h3>Instagram</h3>
        </div>
        <div class="arrow-icon">
          <i class="fas fa-chevron-right"></i>
        </div>
      </a>
      
      <!-- YouTube Button -->
      <a class="action-btn btn-youtube" href="https://www.youtube.com/@ksdigitalservice" target="_blank">
        <div class="btn-icon">
          <i class="fab fa-youtube"></i>
        </div>
        <div class="btn-content">
          <h3>YouTube Channel</h3>
        </div>
        <div class="arrow-icon">
          <i class="fas fa-chevron-right"></i>
        </div>
      </a>
      
      <!-- Self Printer Button 
      <a class="action-btn btn-printer" href="https://ksdigitalservice.pw/print/1" target="_blank">
        <div class="btn-icon">
          <i class="fas fa-print"></i>
        </div>
        <div class="btn-content">
          <h3>Self Printer Portal</h3>
          <p>Access our online printing services and tools</p>
        </div>
        <div class="arrow-icon">
          <i class="fas fa-chevron-right"></i>
        </div>
      </a>
      -->
    </div>
    
    <div class="contact-info">
      <p><i class="fas fa-clock"></i> Business Hours: 7:00 AM - 10:00 PM</p>
      <p><i class="fas fa-envelope"></i> Email: ksdigital2025@gmail.com</p>
      <p class="phone-number">
        <i class="fas fa-phone"></i> +91 78938 45696
      </p>
    </div>
  </div>
</main>

<footer>
  <div class="footer-content">
    <p>© 2025 KS Digital Services. All rights reserved.</p>
    <p>Providing reliable digital solutions for businesses and individuals.</p>
    <p class="copyright">Designed with <i class="fas fa-heart" style="color:#e74c3c;"></i> for our valued customers</p>
  </div>
</footer>

</body>
</html>

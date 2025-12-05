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
  --radius: 8px;
  --shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
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
  background: #f8f9fa;
  color: var(--dark);
  line-height: 1.5;
  min-height: 100vh;
  padding: 1rem;
}

/* Main Container */
.container {
  max-width: 900px;
  margin: 0 auto;
  background: white;
  border-radius: 12px;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  padding: 1.5rem;
}

/* Title Section - Minimal Gap */
.title-section {
  text-align: center;
  margin-bottom: 1rem; /* Reduced gap */
}

h1 {
  font-family: 'Playfair Display', serif;
  font-size: 2.5rem;
  font-weight: 700;
  color: var(--primary);
  margin-bottom: 0.3rem; /* Very small gap */
  padding-bottom: 0.5rem;
  border-bottom: 2px solid var(--gold);
  display: inline-block;
}

/* Main Page Button - Minimal Gap */
.main-page-btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  background: #2ecc71;
  color: white;
  padding: 0.6rem 1.5rem;
  border-radius: 6px;
  text-decoration: none;
  font-weight: 500;
  font-size: 0.9rem;
  margin: 0; /* No margin */
  transition: var(--transition);
}

.main-page-btn:hover {
  background: #27ae60;
  transform: translateY(-2px);
}

/* Contact Buttons Row - Single Line */
.contact-buttons-row {
  display: flex;
  gap: 1rem;
  justify-content: center;
  margin: 1.5rem 0; /* Reduced margin */
  flex-wrap: wrap;
}

.contact-btn {
  flex: 1;
  min-width: 140px;
  background: white;
  border: 1px solid #e0e0e0;
  border-radius: var(--radius);
  padding: 0.8rem 1rem;
  text-decoration: none;
  color: var(--dark);
  display: flex;
  align-items: center;
  gap: 0.8rem;
  transition: var(--transition);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
}

.contact-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
  border-color: var(--secondary);
}

.btn-icon {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1rem;
  color: white;
  flex-shrink: 0;
}

.btn-content h3 {
  font-size: 0.95rem;
  margin-bottom: 0.1rem;
  color: var(--primary);
  font-weight: 600;
}

.btn-content p {
  font-size: 0.8rem;
  color: var(--gray);
}

/* Color variations */
.btn-call .btn-icon { background: #2ecc71; }
.btn-maps .btn-icon { background: var(--secondary); }
.btn-whatsapp .btn-icon { background: #25D366; }

/* Offerings List - Clean and Simple */
.offerings-section {
  margin: 2rem 0;
}

.offerings-section h2 {
  font-family: 'Inter', sans-serif;
  font-size: 1.4rem;
  color: var(--primary);
  text-align: center;
  margin-bottom: 1.2rem;
  font-weight: 600;
}

.offerings-list {
  list-style: none;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 0.6rem;
}

.offerings-list li {
  padding: 0.6rem 0.8rem;
  background: #f8f9fa;
  border-radius: 6px;
  font-size: 0.9rem;
  color: var(--dark);
  transition: var(--transition);
  position: relative;
  padding-left: 2.2rem;
  border-left: 3px solid transparent;
}

.offerings-list li:hover {
  background: #e9ecef;
  border-left-color: var(--secondary);
}

.offerings-list li::before {
  content: '•';
  position: absolute;
  left: 0.8rem;
  color: var(--secondary);
  font-size: 1.2rem;
}

/* Contact Info */
.contact-info {
  background: #f8f9fa;
  border-radius: var(--radius);
  padding: 1.5rem;
  margin: 2rem 0;
  text-align: center;
  border-top: 2px solid var(--gold);
}

.contact-info h2 {
  font-family: 'Inter', sans-serif;
  font-size: 1.3rem;
  color: var(--primary);
  margin-bottom: 1rem;
  font-weight: 600;
}

.contact-details {
  display: flex;
  flex-direction: column;
  gap: 0.8rem;
}

.contact-item {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.6rem;
  color: var(--gray);
  font-size: 0.95rem;
}

.contact-item i {
  color: var(--secondary);
  width: 20px;
}

.phone-number {
  font-size: 1.1rem;
  color: var(--primary);
  font-weight: 600;
  margin-top: 0.3rem;
}

/* Footer */
footer {
  text-align: center;
  padding: 1.5rem 1rem;
  color: var(--gray);
  font-size: 0.85rem;
  background: var(--primary);
  color: rgba(255, 255, 255, 0.85);
  border-radius: 8px;
  margin-top: 1rem;
}

.footer-content {
  max-width: 900px;
  margin: 0 auto;
}

.copyright {
  margin-top: 0.8rem;
  font-size: 0.75rem;
  color: rgba(255, 255, 255, 0.6);
}

/* Responsive Design */
@media (max-width: 768px) {
  body {
    padding: 0.5rem;
  }
  
  .container {
    padding: 1rem;
  }
  
  h1 {
    font-size: 2rem;
  }
  
  .contact-buttons-row {
    flex-direction: column;
    gap: 0.8rem;
  }
  
  .contact-btn {
    width: 100%;
    min-width: 100%;
  }
  
  .offerings-list {
    grid-template-columns: 1fr;
    gap: 0.5rem;
  }
  
  .contact-info {
    padding: 1.2rem;
  }
}

@media (max-width: 480px) {
  h1 {
    font-size: 1.7rem;
  }
  
  .main-page-btn {
    padding: 0.5rem 1.2rem;
    font-size: 0.85rem;
  }
  
  .offerings-list li {
    padding: 0.5rem 0.7rem;
    padding-left: 2rem;
    font-size: 0.85rem;
  }
  
  .contact-btn {
    padding: 0.7rem;
  }
  
  .btn-icon {
    width: 36px;
    height: 36px;
    font-size: 0.9rem;
  }
}
</style>

</head>
<body>

<div class="container">
  <!-- 1. KS DIGITAL SERVICES Title -->
  <div class="title-section">
    <h1>KS DIGITAL SERVICES</h1>
    
    <!-- 2. Main Page Link Button - MINIMAL GAP -->
    <a class="main-page-btn" href="https://ksdigitalservice.pw/">
      <i class="fas fa-home"></i>
      Main Page
    </a>
  </div>
  
  <!-- 3. Call, Get Directions, WhatsApp Buttons in SINGLE LINE -->
  <div class="contact-buttons-row">
    <a class="contact-btn btn-call" href="tel:+917893845696">
      <div class="btn-icon">
        <i class="fas fa-phone-alt"></i>
      </div>
      <div class="btn-content">
        <h3>Call Now</h3>
        <p>+91 78938 45696</p>
      </div>
    </a>
    
    <a class="contact-btn btn-maps" href="https://maps.app.goo.gl/VfZ4fHYw6nYFTavB6" target="_blank">
      <div class="btn-icon">
        <i class="fas fa-map-marker-alt"></i>
      </div>
      <div class="btn-content">
        <h3>Get Directions</h3>
        <p>Find Location</p>
      </div>
    </a>
    
    <a class="contact-btn btn-whatsapp" href="https://wa.me/7893845696" target="_blank">
      <div class="btn-icon">
        <i class="fab fa-whatsapp"></i>
      </div>
      <div class="btn-content">
        <h3>WhatsApp</h3>
        <p>Chat with Us</p>
      </div>
    </a>
  </div>
  
  <!-- 4. Offerings as a Clean List -->
  <div class="offerings-section">
    <h2>Our Services & Offerings</h2>
    <ul class="offerings-list">
      <li>FSSAI / Trade / Labor License</li>
      <li>GST Registration / Returns</li>
      <li>ITR Filing (Income Tax)</li>
      <li>PF (EPFO) Services</li>
      <li>Passport / PAN Card / Voter ID</li>
      <li>AEPS Money Withdrawal</li>
      <li>Credit Card to Bank Transfer</li>
      <li>Aadhar Address Change</li>
      <li>Train / Bus / Flight Ticket Bookings</li>
      <li>All Entrance Exams Applications</li>
      <li>Insurance & Bank A/C Opening</li>
      <li>Plastic PVC Card Printing</li>
      <li>Project Works / Resume Making</li>
      <li>Document Editing</li>
      <li>Rental Agreement</li>
      <li>Scholarships Fresh / Renewal</li>
      <li>Tally ERP Services</li>
      <li>PM Vishwakarma, ABHA, PMEGP</li>
      <li>Senior Citizen (Aasara Card)</li>
      <li>DOST Application & TTD Bookings</li>
      <li>Property Tax / Electricity Bill Payment</li>
    </ul>
  </div>
  
  <!-- 5. Contact Info -->
  <div class="contact-info">
    <h2>Contact Information</h2>
    <div class="contact-details">
      <div class="contact-item">
        <i class="fas fa-clock"></i>
        <span>Business Hours: 7:00 AM - 10:00 PM</span>
      </div>
      <div class="contact-item">
        <i class="fas fa-envelope"></i>
        <span>Email: ksdigital2025@gmail.com</span>
      </div>
      <div class="contact-item phone-number">
        <i class="fas fa-phone"></i>
        <span>+91 78938 45696</span>
      </div>
    </div>
  </div>
</div>

<!-- 6. Footer -->
<footer>
  <div class="footer-content">
    <p>© 2025 KS Digital Services. All rights reserved.</p>
    <p>Providing reliable digital solutions for businesses and individuals.</p>
    <p class="copyright">Designed for our valued customers</p>
  </div>
</footer>

</body>
</html>

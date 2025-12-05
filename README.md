<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>KS DIGITAL SERVICES</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
/* Reset and Base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  -webkit-tap-highlight-color: transparent;
}

body {
  font-family: 'Inter', sans-serif;
  background: #ffffff;
  color: #333333;
  line-height: 1.4;
  min-height: 100vh;
  padding: 15px;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100%;
  overflow-x: hidden;
}

/* Main Container */
.container {
  max-width: 100%;
  margin: 0 auto;
  background: #ffffff;
  overflow: hidden;
  width: 100%;
}

/* Left-aligned Title */
.title-section {
  text-align: left;
  margin-bottom: 15px;
  width: 100%;
  padding: 0 5px;
}

h2 {
  font-family: 'Poppins', sans-serif;
  font-size: 12px;
  font-weight: 700;
  color: #2c3e50;
  margin-bottom: 8px;
  text-align: left;
  border-bottom: none;
  width: 100%;
}

/* First row buttons: Main Page + Call Now */
.button-row-1 {
  display: flex;
  gap: 10px;
  margin-bottom: 15px;
  width: 100%;
  flex-wrap: nowrap;
}

/* Second row buttons: Get Directions + WhatsApp */
.button-row-2 {
  display: flex;
  gap: 10px;
  margin-bottom: 20px;
  width: 100%;
  flex-wrap: nowrap;
}

/* Button styles */
.action-btn {
  flex: 1;
  min-width: 0;
  background: white;
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  padding: 12px 8px;
  text-decoration: none;
  color: #333;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.2s;
  box-shadow: 0 2px 5px rgba(0,0,0,0.05);
  text-align: center;
  font-size: 22px;
  font-weight: 500;
}

.action-btn:active {
  transform: scale(0.98);
  box-shadow: 0 1px 3px rgba(0,0,0,0.1);
}

/* Main Page button specific */
.main-page-btn {
  background: #27ae60;
  color: white;
  border: none;
  padding: 12px 15px;
}

.main-page-btn i {
  margin-right: 5px;
}

/* Call Now button specific */
.call-btn {
  background: #f0f9ff;
  border-color: #3498db;
  color: #2c3e50;
}

.call-btn i {
  color: #27ae60;
  margin-right: 5px;
}

/* Maps button specific */
.maps-btn {
  background: #f0f9ff;
  border-color: #3498db;
  color: #2c3e50;
}

.maps-btn i {
  color: #3498db;
  margin-right: 5px;
}

/* WhatsApp button specific */
.whatsapp-btn {
  background: #f0f9ff;
  border-color: #25D366;
  color: #2c3e50;
}

.whatsapp-btn i {
  color: #25D366;
  margin-right: 5px;
}

/* Left-aligned Offerings */
.offerings-section {
  margin: 20px 0;
  width: 100%;
  padding: 0;
}

.section-title {
  font-family: 'Poppins', sans-serif;
  font-size: 20px;
  font-weight: 600;
  color: #2c3e50;
  text-align: left;
  margin-bottom: 15px;
  padding-bottom: 5px;
  border-bottom: 2px solid #3498db;
  width: 100%;
  padding-left: 0;
  margin-left: 0;
}

.offerings-list {
  list-style: none;
  margin: 0;
  padding: 0;
  display: grid;
  grid-template-columns: 1fr;
  gap: 8px;
  width: 100%;
}

.offerings-list li {
  padding: 10px 15px;
  background: #f8f9fa;
  border-radius: 6px;
  font-size: 14px;
  color: #444;
  text-align: left;
  width: 100%;
  margin-left: 0;
}

/* Left-aligned Contact Info */
.contact-info {
  background: #f8f9fa;
  border-radius: 10px;
  padding: 15px;
  margin: 20px 0;
  border-top: 2px solid #3498db;
  width: 100%;
  box-sizing: border-box;
}

.contact-info h3 {
  font-family: 'Poppins', sans-serif;
  font-size: 18px;
  color: #2c3e50;
  margin-bottom: 12px;
  text-align: left;
  font-weight: 600;
}

.contact-details {
  display: flex;
  flex-direction: column;
  gap: 10px;
  text-align: left;
}

.contact-item {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  color: #555;
  font-size: 14px;
  text-align: left;
}

.contact-item i {
  color: #3498db;
  width: 20px;
  font-size: 14px;
  flex-shrink: 0;
}

.phone-number {
  font-size: 15px;
  color: #2c3e50;
  font-weight: 600;
  margin-top: 5px;
}

/* Footer */
footer {
  text-align: center;
  padding: 15px;
  color: #666;
  font-size: 12px;
  background: #f8f9fa;
  border-radius: 8px;
  margin-top: 15px;
  width: 100%;
  box-sizing: border-box;
}

.footer-content p {
  margin-bottom: 5px;
}

.copyright {
  font-size: 11px;
  color: #888;
  margin-top: 8px;
}

/* Mobile-specific adjustments */
@media (max-width: 480px) {
  body {
    padding: 12px;
  }
  
  h2 {
    font-size: 12px;
    text-align: left;
  }
  
  .button-row-1, .button-row-2 {
    gap: 8px;
  }
  
  .action-btn {
    padding: 10px 6px;
    font-size: 18px;
  }
  
  .section-title {
    font-size: 18px;
    padding-left: 0;
    margin-left: 0;
  }
  
  .offerings-list li {
    font-size: 15px;
    text-align: left;
    padding: 10px 15px;
    margin-left: 0;
  }
  
  .main-page-btn {
    padding: 10px 12px;
  }
  
  .contact-info h3 {
    font-size: 16px;
  }
}

@media (max-width: 350px) {
  h2 {
    font-size: 12px;
    text-align: left;
  }
  
  .button-row-1, .button-row-2 {
    gap: 6px;
  }
  
  .action-btn {
    padding: 8px 4px;
    font-size: 18px;
  }
  
  .section-title {
    padding-left: 0;
    margin-left: 0;
  }
  
  .offerings-list li {
    font-size: 12px;
    text-align: left;
    padding: 10px 15px;
    margin-left: 0;
  }
}

/* Ensure no overflow */
html, body, .container, .title-section, .offerings-section, .contact-info {
  max-width: 100%;
  overflow-x: hidden;
}

/* Touch-friendly buttons */
button, a {
  cursor: pointer;
  -webkit-user-select: none;
  user-select: none;
}

/* Clear any floating elements */
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}
</style>

</head>
<body>

<div class="container">
  <!-- KS DIGITAL SERVICES Title - Left aligned -->
  <div class="title-section">
    <h2>KS DIGITAL SERVICES</h2>
    
    <!-- First row: Main Page + Call Now -->
    <div class="button-row-1">
      <a class="action-btn main-page-btn" href="https://ksdigitalservice.pw/">
        <i class="fas fa-home"></i> Main Page
      </a>
      <a class="action-btn call-btn" href="tel:+917893845696">
        <i class="fas fa-phone-alt"></i> Call Now
      </a>
    </div>
    
    <!-- Second row: Get Directions + WhatsApp -->
    <div class="button-row-2">
      <a class="action-btn maps-btn" href="https://maps.app.goo.gl/VfZ4fHYw6nYFTavB6" target="_blank">
        <i class="fas fa-map-marker-alt"></i> Get Directions
      </a>
      <a class="action-btn whatsapp-btn" href="https://wa.me/7893845696" target="_blank">
        <i class="fab fa-whatsapp"></i> WhatsApp
      </a>
    </div>
  </div>
  
  <!-- Offerings as a List - Left aligned -->
  <div class="offerings-section">
    <h2 class="section-title">Our Services & Offerings</h2>
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
  
  <!-- Contact Info - Left aligned -->
  <div class="contact-info">
    <h3>Contact Information</h3>
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

<!-- Footer -->
<footer>
  <div class="footer-content">
    <p>© 2025 KS Digital Services</p>
    <p>Providing reliable digital solutions</p>
    <p class="copyright">Designed for mobile users</p>
  </div>
</footer>

</body>
</html>

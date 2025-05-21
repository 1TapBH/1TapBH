<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>1 Tap BH – One Tap to All Your Needs</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #000;
      color: gold;
      scroll-behavior: smooth;
    }
    header {
      text-align: center;
      padding: 60px 20px;
      background-color: #111;
      animation: fadeIn 1s ease-out;
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
    }
    header p {
      font-size: 1.2rem;
      color: #ccc;
    }
    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
      animation: fadeIn 1.5s ease-out;
    }
    h2 {
      color: gold;
    }
    .features, .how-it-works, .pricing {
      margin-top: 40px;
    }
    .feature-item, .step-item, .price-plan {
      background-color: #1a1a1a;
      margin: 20px 0;
      padding: 20px;
      border-radius: 10px;
      transition: transform 0.3s ease;
    }
    .feature-item:hover, .step-item:hover, .price-plan:hover {
      transform: scale(1.02);
    }
    footer {
      text-align: center;
      padding: 30px;
      background-color: #111;
      color: #aaa;
    }
    a {
      color: gold;
      text-decoration: none;
    }
    .demo-card {
      background-color: #1a1a1a;
      padding: 20px;
      border-radius: 15px;
      text-align: center;
      margin-top: 30px;
    }
    .demo-card h3 {
      margin: 10px 0;
    }
    .demo-card a {
      display: block;
      margin: 10px 0;
      padding: 10px;
      background-color: #333;
      border-radius: 8px;
    }
    .form-group {
      margin: 10px 0;
    }
    input[type="text"], input[type="email"] {
      width: 100%;
      padding: 10px;
      border-radius: 6px;
      border: none;
      background-color: #222;
      color: gold;
    }
    button {
      margin-top: 20px;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      background-color: gold;
      color: black;
      font-weight: bold;
      cursor: pointer;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <h1>1 Tap BH</h1>
    <p>One Tap to All Your Needs</p>
  </header>  <section class="features">
    <h2>Features</h2>
    <div class="feature-item">NFC-enabled smart business cards</div>
    <div class="feature-item">QR Code contact sharing</div>
    <div class="feature-item">Customizable Linktree-style profiles</div>
    <div class="feature-item">Instant contact saving to phone</div>
  </section>  <section class="how-it-works">
    <h2>How It Works</h2>
    <div class="step-item">1. Tap your 1 Tap BH card on any phone</div>
    <div class="step-item">2. Your digital profile appears instantly</div>
    <div class="step-item">3. Contact is saved or shared in seconds</div>
  </section>  <section class="pricing">
    <h2>Pricing</h2>
    <div class="price-plan">Basic Profile – Free</div>
    <div class="price-plan">Premium NFC Card – 20 BHD (One-time)</div>
    <div class="price-plan">Pro Analytics & Branding – 2 BHD/month</div>
  </section>  <section>
    <h2>Create Your Profile</h2>
    <div class="form-group"><input type="text" id="name" placeholder="Your Name"></div>
    <div class="form-group"><input type="text" id="phone" placeholder="Phone Number"></div>
    <div class="form-group"><input type="email" id="email" placeholder="Email"></div>
    <div class="form-group"><input type="text" id="instagram" placeholder="Instagram Link"></div>
    <div class="form-group"><input type="text" id="whatsapp" placeholder="WhatsApp Link"></div>
    <div class="form-group"><input type="text" id="linktree" placeholder="Linktree URL"></div>
    <button onclick="generateProfile()">Generate Preview</button><div class="demo-card" id="generatedCard" style="display:none;">
  <h3 id="cardName"></h3>
  <a href="#" id="cardWhatsApp">WhatsApp</a>
  <a href="#" id="cardInstagram">Instagram</a>
  <a href="#" id="cardEmail">Email</a>
  <a href="#" id="cardLinktree">Full Profile</a>
</div>

  </section>  <section>
    <h2>Contact Us</h2>
    <p>WhatsApp: <a href="https://wa.me/97336145412">+973 3614 5412</a></p>
    <p>Instagram: <a href="https://instagram.com/1tapbh">@1tapbh</a></p>
  </section>  <footer>
    &copy; 2025 1 Tap BH. All rights reserved.
  </footer>  <script>
    function generateProfile() {
      const name = document.getElementById('name').value;
      const phone = document.getElementById('phone').value;
      const email = document.getElementById('email').value;
      const instagram = document.getElementById('instagram').value;
      const whatsapp = document.getElementById('whatsapp').value;
      const linktree = document.getElementById('linktree').value;

      document.getElementById('cardName').innerText = name;
      document.getElementById('cardWhatsApp').href = whatsapp;
      document.getElementById('cardInstagram').href = instagram;
      document.getElementById('cardEmail').href = `mailto:${email}`;
      document.getElementById('cardLinktree').href = linktree;

      document.getElementById('generatedCard').style.display = 'block';
    }
  </script></body>
</html>

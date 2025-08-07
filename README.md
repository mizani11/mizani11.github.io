# mizanitz.github.io
Welcome <!DOCTYPE html>
<html lang="sw">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mizani Tz - Mizani Bora Kisutu, Dar es Salaam</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <div class="container">
      <h1>Mizani Tz</h1>
      <nav>
        <button id="lang-sw" class="lang-btn active">Kiswahili</button>
        <button id="lang-en" class="lang-btn">English</button>
      </nav>
    </div>
  </header>

  <section class="hero">
    <div class="container">
      <h2 class="sw">Karibu Mizani Tz – Wataalamu wa Mizani ya Kisasa kwa Biashara Yako!</h2>
      <h2 class="en" style="display:none">Welcome to Mizani Tz – Precision Weighing Solutions for Every Business!</h2>
      <p class="sw">
        Tunauza aina zote za mizani – kutoka madukani hadi viwandani.<br />
        Ubora wa hali ya juu, huduma ya haraka, na bei nafuu!
      </p>
      <p class="en" style="display:none">
        We sell all types of weighing scales – from retail to industrial.<br />
        High quality, fast service, and affordable prices!
      </p>
      <a href="#contact" class="btn">Wasiliana Nasi</a>
    </div>
  </section>

  <section class="services container">
    <h3 class="sw">Huduma Zetu</h3>
    <h3 class="en" style="display:none">Our Services</h3>
    <div class="service-grid">
      <div class="service-item">
        <img src="images/retail-scale.jpg" alt="Mizani ya Madukani" />
        <h4 class="sw">Mizani ya Madukani</h4>
        <h4 class="en" style="display:none">Retail Scales</h4>
      </div>
      <div class="service-item">
        <img src="images/market-scale.jpg" alt="Mizani ya Sokoni" />
        <h4 class="sw">Mizani ya Sokoni</h4>
        <h4 class="en" style="display:none">Market Scales</h4>
      </div>
      <div class="service-item">
        <img src="images/industrial-scale.jpg" alt="Mizani ya Viwandani" />
        <h4 class="sw">Mizani ya Viwandani</h4>
        <h4 class="en" style="display:none">Industrial Scales</h4>
      </div>
      <div class="service-item">
        <img src="images/digital-scale.jpg" alt="Mizani za Digitali na Counting" />
        <h4 class="sw">Mizani za Digitali na Counting</h4>
        <h4 class="en" style="display:none">Digital & Counting Scales</h4>
      </div>
      <div class="service-item">
        <img src="images/livestock-scale.jpg" alt="Mizani ya Wanyama na Mifugo" />
        <h4 class="sw">Mizani ya Wanyama na Mifugo</h4>
        <h4 class="en" style="display:none">Livestock & Animal Scales</h4>
      </div>
      <div class="service-item">
        <img src="images/crane-scale.jpg" alt="Mizani za Crane na Pallet" />
        <h4 class="sw">Mizani za Crane na Pallet</h4>
        <h4 class="en" style="display:none">Crane & Pallet Scales</h4>
      </div>
    </div>
  </section>

  <section class="contact container" id="contact">
    <h3 class="sw">Wasiliana Nasi</h3>
    <h3 class="en" style="display:none">Contact Us</h3>
    <form id="contactForm">
      <label class="sw" for="name">Jina:</label>
      <label class="en" style="display:none" for="name">Name:</label>
      <input type="text" id="name" name="name" required />

      <label class="sw" for="email">Barua Pepe:</label>
      <label class="en" style="display:none" for="email">Email:</label>
      <input type="email" id="email" name="email" required />

      <label class="sw" for="message">Ujumbe:</label>
      <label class="en" style="display:none" for="message">Message:</label>
      <textarea id="message" name="message" rows="5" required></textarea>

      <button type="submit" class="btn sw">Tuma</button>
      <button type="submit" class="btn en" style="display:none">Send</button>
    </form>
    <p id="formMessage"></p>
  </section>

  <footer>
    <div class="container footer-content">
      <p>Mizani Tz &copy; 2025 | Kisutu, Dar es Salaam</p>
      <p>Simu: 0789 617373 | 0719 617373 | 0769 617373</p>
      <p><a href="https://wa.me/0789617373" target="_blank">Tuma WhatsApp</a></p>
    </div>
  </footer>

  <button id="whatsappBtn" title="Wasiliana kwa WhatsApp">📱</button>

  <script src="script.js"></script>
</body>
</html>/* Reset & Base */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background: #f8f9fa;
  color: #333;
  line-height: 1.6;
}
.container {
  max-width: 1100px;
  margin: auto;
  padding: 0 20px;
}
header {
  background: #004d40;
  color: #fff;
  padding: 15px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
header h1 {
  margin-left: 10px;
  font-size: 24px;
}
nav {
  margin-right: 10px;
}
.lang-btn {
  background: transparent;
  border: 1.5px solid #fff;
  color: #fff;
  padding: 5px 10px;
  margin-left: 5px;
  cursor: pointer;
  border-radius: 4px;
  font-weight: bold;
}
.lang-btn.active {
  background: #00796b;
  border-color: #00796b;
}
.hero {
  background: url('images/scale-banner.jpg') no-repeat center center/cover;
  color: white;
  text-align: center;
  padding: 90px 20px 70px;
  box-shadow: inset 0 0 0 1000px rgba(0,0,0,0.35);
}
.hero h2 {
  font-size: 36px;
  margin-bottom: 15px;
}
.hero p {
  font-size: 18px;
  margin-bottom: 25px;
}
.btn {
  display: inline-block;
  background: #00796b;
  color: white;
  padding: 12px 25px;
  border-radius: 30px;
  text-decoration: none;
  font-weight: bold;
  transition: background 0.3s ease;
  cursor: pointer;
}
.btn:hover {
  background: #004d40;
}
.services {
  margin: 40px 0;
  text-align: center;
}
.services h3 {
  margin-bottom: 30px;
  font-size: 28px;
  color: #004d40;
}
.service-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(200px,1fr));
  gap: 25px;
}
.service-item {
  background: white;
  border-radius: 12px;
  padding: 15px;
  box-shadow: 0 2px 7px rgba(0,0,0,0.1);
  transition: transform 0.3s ease;
}
.service-item:hover {
  transform: translateY(-5px);
}
.service-item img {
  max-width: 100%;
  border-radius: 12px;
  margin-bottom: 10px;
}
.service-item h4 {
  color: #00796b;
  font-weight: bold;
}
.contact {
  background: #e0f2f1;
  padding: 30px 20px 50px;
  border-radius: 12px;
  margin-bottom: 30px;
}
.contact h3 {
  text-align: center;
  margin-bottom: 20px;
  color: #004d40;
}
form label {
  display: block;
  margin: 10px 0 5px;
  font-weight: bold;
}
form input, form textarea {
  width: 100%;
  padding: 8px 12px;
  border-radius: 6px;
  border: 1.5px solid #00796b;
  resize: vertical;
}
form button {
  margin-top: 15px;
  width: 100%;
}
footer {
  background: #004d40;
  color: #fff;
  padding: 18px 20px;
  text-align: center;
  font-size: 14px;
}
.footer-content p {
  margin: 5px 0;
}
#whatsappBtn {
  position: fixed;
  bottom: 25px;
  right: 25px;
  background: #25d366;
  border: none;
  border-radius: 50%;
  padding: 15px 18px;
  font-size: 28px;
  color: white;
  cursor: pointer;
  box-shadow: 0 5px 10px rgba(0,0,0,0.3);
  transition: background 0.3s ease;
  z-index: 9999;
}
#whatsappBtn:hover {
  background: #128c4a;
}
@media (max-width: 600px) {
  .hero h2 {
    font-size: 26px;
  }
  .services h3 {
    font-size: 22px;
  }
}// Language switcher
const langSwBtn = document.getElementById('lang-sw');
const langEnBtn = document.getElementById('lang-en');

langSwBtn.addEventListener('click', () => {
  setLanguage('sw');
});
langEnBtn.addEventListener('click', () => {
  setLanguage('en');
});

function setLanguage(lang) {
  if (lang === 'sw') {
    document.querySelectorAll('.sw').forEach(el => el.style.display = '');
    document.querySelectorAll('.en').forEach(el => el.style.display = 'none');
    langSwBtn.classList.add('active');
    langEnBtn.classList.remove('active');
  } else {
    document.querySelectorAll('.sw').forEach(el => el.style.display = 'none');
    document.querySelectorAll('.en').forEach(el => el.style.display = '');
    langSwBtn.classList.remove('active');
    langEnBtn.classList.add('active');
  }
}

// WhatsApp Button
const whatsappBtn = document.getElementById('whatsappBtn');
whatsappBtn.addEventListener('click', () => {
  // Choose one number to open chat with (first one here)
  window.open('https://wa.me/0789617373', '_blank');
});

// Contact Form submission
const contactForm = document.getElementById('contactForm');
const formMessage = document.getElementById('formMessage');

contactForm.addEventListener('submit', e => {
  e.preventDefault();

  // Basic validation
  const name = contactForm.name.value.trim();
  const email = contactForm.email.value.trim();
  const message = contactForm.message.value.trim();

  if (!name || !email || !message) {
    formMessage.style.color = 'red';
    formMessage.textContent = 'Tafadhali jaza sehemu zote.';
    return;
  }

  // Since no backend, just simulate success message
  formMessage.style.color = 'green';
  formMessage.textContent = 'Ujumbe wako umetumwa! Tutakujibu hivi karibuni.';

  contactForm.reset();
});

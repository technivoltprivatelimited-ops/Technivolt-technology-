# Technivolt-technology-
Employment agency 
 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Technivolt Technologies</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    * {margin:0; padding:0; box-sizing:border-box; font-family: 'Roboto', sans-serif;}
    body {background:#f5f7fa; color:#333;}
    header {background:#007BFF; color:#fff; padding:20px 0; text-align:center;}
    header h1 {margin-bottom:5px;}
    nav a {color:#fff; margin:0 15px; text-decoration:none; font-weight:500;}
    nav a:hover {text-decoration:underline;}
    section {padding:60px 20px; max-width:1100px; margin:0 auto;}
    h2 {color:#007BFF; margin-bottom:20px; text-align:center;}
    p {line-height:1.6; margin-bottom:15px;}
    .services, .portfolio {display:flex; flex-wrap:wrap; gap:20px; justify-content:center;}
    .card {background:#fff; padding:20px; border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1); flex:1 1 250px; text-align:center;}
    .btn {background:#007BFF; color:#fff; padding:12px 25px; border:none; border-radius:8px; cursor:pointer; text-decoration:none;}
    .btn:hover {background:#0056b3;}
    footer {background:#222; color:#fff; padding:20px 0; text-align:center;}
    /* Image slider */
    .slider {position:relative; overflow:hidden; max-width:100%; margin-bottom:40px;}
    .slides {display:flex; transition:0.5s ease;}
    .slides img {width:100%; border-radius:12px;}
    .slider-buttons {position:absolute; top:50%; width:100%; display:flex; justify-content:space-between; transform:translateY(-50%);}
    .slider-buttons button {background:rgba(0,0,0,0.5); color:#fff; border:none; padding:10px; cursor:pointer; border-radius:50%;}
    /* WhatsApp button */
    .whatsapp {position:fixed; bottom:20px; right:20px; background:#25D366; color:#fff; padding:15px 20px; border-radius:50px; text-decoration:none; font-weight:bold; box-shadow:0 4px 8px rgba(0,0,0,0.2);}
  </style>
</head>
<body>

<header>
  <h1>Technivolt Technologies</h1>
  <p>Your Trusted Employment Agency</p>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About Us</a>
    <a href="#services">Services</a>
    <a href="#portfolio">Portfolio</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<section id="home">
  <h2>We Provide Jobs</h2>
  <p>Looking for reliable work? We provide jobs like Captcha Typing, Data Entry, Online Typing, PDF Typing, Handwriting, and more.</p>
  <div class="slider">
    <div class="slides">
      <img src="https://via.placeholder.com/1100x400?text=Captcha+Typing+Work" alt="Captcha Typing">
      <img src="https://via.placeholder.com/1100x400?text=Data+Entry+Work" alt="Data Entry">
      <img src="https://via.placeholder.com/1100x400?text=Online+Typing+Work" alt="Online Typing">
    </div>
    <div class="slider-buttons">
      <button id="prev">&#10094;</button>
      <button id="next">&#10095;</button>
    </div>
  </div>
</section>

<section id="about">
  <h2>About Us</h2>
  <p>Technivolt Technologies is a trusted employment agency providing work-from-home and office-based opportunities. We connect talented individuals with top companies to help them achieve their career goals.</p>
</section>

<section id="services">
  <h2>Our Services</h2>
  <div class="services">
    <div class="card"><h3>Work From Home</h3><p>Flexible remote work opportunities like data entry, typing, and online work.</p></div>
    <div class="card"><h3>Work From Office</h3><p>Professional in-office work with top companies and secure employment.</p></div>
  </div>
</section>

<section id="portfolio">
  <h2>Our Partners</h2>
  <div class="portfolio">
    <div class="card"><h3>Amazon</h3></div>
    <div class="card"><h3>Flipkart</h3></div>
    <div class="card"><h3>Databrilla</h3></div>
    <div class="card"><h3>HDFC</h3></div>
    <div class="card"><h3>Bajaj Finance</h3></div>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <p>Address: Technivolt Technologies, Second Floor Vikas Apartment, Prushottam Gali B Wink, Prabhat Devi, Mumbai, Maharashtra 400026</p>
  <p>Email: <a href="mailto:info@technivolt.com">info@technivolt.com</a></p>
  <p>WhatsApp: <a href="https://wa.me/911234567890" target="_blank">+91 12345 67890</a></p>
</section>

<a href="https://wa.me/911234567890" class="whatsapp" target="_blank">WhatsApp Us</a>

<footer>
  <p>&copy; 2025 Technivolt Technologies. All Rights Reserved.</p>
</footer>

<script>
  // Slider functionality
  const slides = document.querySelector('.slides');
  const slideImages = document.querySelectorAll('.slides img');
  let index = 0;

  document.getElementById('next').addEventListener('click', () => {
    index = (index + 1) % slideImages.length;
    slides.style.transform = `translateX(-${index * 100}%)`;
  });
  document.getElementById('prev').addEventListener('click', () => {
    index = (index - 1 + slideImages.length) % slideImages.length;
    slides.style.transform = `translateX(-${index * 100}%)`;
  });
</script>

</body>
</html>
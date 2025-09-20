
<!doctype html>
<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Snp Mart - Online Store</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#06b6d4; --text:#e6eef6;
      --muted:#9fb3c7; --radius:12px;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, system-ui, Arial;background:linear-gradient(180deg,#071023 0%, var(--bg) 100%);color:var(--text);line-height:1.5}
    .wrap{max-width:1000px;margin:40px auto;padding:24px}
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:28px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:700}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600}
    .hero{padding:50px 20px;text-align:center}
    .hero h1{font-size:32px;margin:0 0 12px}
    .hero p{color:var(--muted);margin:0 0 18px}
    .btn{display:inline-block;padding:10px 16px;border-radius:10px;background:var(--accent);color:#042027;text-decoration:none;font-weight:700}
    .card{background:rgba(255,255,255,0.02);border:1px solid rgba(255,255,255,0.04);padding:18px;border-radius:var(--radius)}
    .products{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px;margin:22px 0}
    .product{padding:14px;border-radius:10px;background:rgba(255,255,255,0.01);border:1px solid rgba(255,255,255,0.05);text-align:center}
    .product img{width:100%;border-radius:8px;margin-bottom:10px}
    footer{margin-top:36px;color:var(--muted);font-size:14px;text-align:center}
    .contact form{display:flex;flex-direction:column;gap:8px}
    input,textarea{padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:var(--text)}
    textarea{min-height:100px;resize:vertical}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">SM</div>
        <div>
          <div style="font-weight:700">Snp Mart</div>
          <div style="font-size:13px;color:var(--muted)">Best Online Store</div>
        </div>
      </div>
      <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <!-- Home -->
    <section id="home" class="hero">
      <h1>Welcome to Snp Mart</h1>
      <p>आपका भरोसेमंद ऑनलाइन स्टोर – Best deals, Best products, Best service</p>
      <a class="btn" href="#products">Shop Now</a>
    </section>

    <!-- Products -->
    <section id="products" class="card">
      <h2>Our Products</h2>
      <div class="products">
        <div class="product">
          <img src="https://via.placeholder.com/200" alt="Product 1">
          <h3>Product 1</h3>
          <p>₹500</p>
          <a href="#" class="btn">Buy</a>
        </div>
        <div class="product">
          <img src="https://via.placeholder.com/200" alt="Product 2">
          <h3>Product 2</h3>
          <p>₹750</p>
          <a href="#" class="btn">Buy</a>
        </div>
        <div class="product">
          <img src="https://via.placeholder.com/200" alt="Product 3">
          <h3>Product 3</h3>
          <p>₹999</p>
          <a href="#" class="btn">Buy</a>
        </div>
      </div>
    </section>

    <!-- About -->
    <section id="about" class="card" style="margin-top:18px">
      <h2>About Us</h2>
      <p style="color:var(--muted)">
        Snp Mart आपके लिए लाता है बेहतरीन प्रोडक्ट्स, किफायती दाम और तेज़ डिलीवरी।  
        हमारा लक्ष्य है कि हर ग्राहक को मिले **100% संतुष्टि**।
      </p>
    </section>

    <!-- Contact -->
    <section id="contact" class="card" style="margin-top:18px">
      <h2>Contact Us</h2>
      <div class="contact">
        <form onsubmit="event.preventDefault(); alert('Demo only — Form काम करने के लिए Formspree या Netlify Forms जोड़ें।');">
          <input placeholder="Name" required />
          <input placeholder="Email" type="email" required />
          <textarea placeholder="Your message"></textarea>
          <button class="btn" type="submit" style="margin-top:8px">Send</button>
        </form>
      </div>
    </section>

    <footer>
      © <span id="year"></span> Snp Mart — All Rights Reserved
    </footer>
  </div>

  <script>
    document.getElementById('year').innerText = new Date().getFullYear();
  </script>
</body>
</html>

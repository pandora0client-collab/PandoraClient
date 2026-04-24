[pandora_client_landing_page.html](https://github.com/user-attachments/files/27052404/pandora_client_landing_page.html)
<!DOCTYPE html>
<html lang="pl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Pandora Client</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    * {margin:0;padding:0;box-sizing:border-box;}
    body {
      font-family: 'Inter', sans-serif;
      background: radial-gradient(circle at top, #0f0f0f, #0a0a0a);
      color: white;
      overflow-x: hidden;
    }

    nav {
      display:flex;
      justify-content:space-between;
      align-items:center;
      padding:20px 60px;
      position:fixed;
      width:100%;
      backdrop-filter: blur(10px);
      background: rgba(10,10,10,0.6);
      z-index:1000;
    }

    nav .logo {
      font-family:'Orbitron';
      font-size:22px;
      letter-spacing:2px;
    }

    nav ul {
      display:flex;
      gap:30px;
      list-style:none;
    }

    nav a {
      text-decoration:none;
      color:#aaa;
      transition:0.3s;
    }

    nav a:hover {color:white;}

    .btn {
      padding:10px 20px;
      border-radius:10px;
      cursor:pointer;
      transition:0.3s;
      font-weight:600;
    }

    .btn-primary {
      background: linear-gradient(90deg,#8a2be2,#ff2ea6);
      border:none;
      color:white;
      box-shadow:0 0 15px rgba(255,0,150,0.4);
    }

    .btn-primary:hover {
      transform:translateY(-2px);
      box-shadow:0 0 25px rgba(255,0,150,0.7);
    }

    .btn-outline {
      border:1px solid rgba(255,255,255,0.2);
      background:transparent;
      color:white;
    }

    .btn-outline:hover {
      border-color:#ff2ea6;
      box-shadow:0 0 10px #ff2ea6;
    }

    .hero {
      height:100vh;
      display:flex;
      flex-direction:column;
      justify-content:center;
      align-items:center;
      text-align:center;
      padding:20px;
      position:relative;
    }

    .badge {
      background: rgba(0,255,100,0.1);
      border:1px solid rgba(0,255,100,0.4);
      padding:5px 12px;
      border-radius:20px;
      margin-bottom:20px;
      font-size:14px;
    }

    .badge::before {
      content:'';
      width:8px;
      height:8px;
      background:#00ff66;
      display:inline-block;
      border-radius:50%;
      margin-right:6px;
    }

    .hero h1 {
      font-size:80px;
      font-family:'Orbitron';
      background: linear-gradient(90deg,#8a2be2,#ff2ea6);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
    }

    .hero p {
      margin-top:15px;
      color:#bbb;
      max-width:600px;
    }

    .hero-buttons {
      margin-top:30px;
      display:flex;
      gap:20px;
    }

    .hero-info {
      margin-top:25px;
      font-size:14px;
      color:#777;
    }

    .pricing {
      padding:100px 40px;
      text-align:center;
    }

    .pricing h2 {
      font-size:40px;
      margin-bottom:10px;
    }

    .pricing p {
      color:#aaa;
      margin-bottom:60px;
    }

    .cards {
      display:flex;
      gap:30px;
      justify-content:center;
      flex-wrap:wrap;
    }

    .card {
      background: rgba(255,255,255,0.03);
      border:1px solid rgba(255,255,255,0.08);
      border-radius:20px;
      padding:30px;
      width:280px;
      backdrop-filter: blur(15px);
      transition:0.3s;
    }

    .card:hover {
      transform:translateY(-10px);
      box-shadow:0 0 30px rgba(255,0,150,0.2);
    }

    .card.highlight {
      transform:scale(1.05);
      border:1px solid #ff2ea6;
      box-shadow:0 0 30px rgba(255,0,150,0.4);
    }

    .price {
      font-size:28px;
      margin:15px 0;
    }

    .features {
      text-align:left;
      margin:20px 0;
      font-size:14px;
      color:#ccc;
    }

    .features li {margin:8px 0;}

    .payments {
      font-size:12px;
      color:#666;
      margin-top:10px;
    }

    footer {
      padding:40px;
      text-align:center;
      color:#666;
    }

    @media(max-width:768px){
      .hero h1 {font-size:50px;}
      nav ul {display:none;}
    }
  </style>
</head>
<body>

<nav>
  <div class="logo">PANDORA</div>
  <ul>
    <li><a href="#">Strona główna</a></li>
    <li><a href="#">Funkcje</a></li>
    <li><a href="#">Zespół</a></li>
    <li><a href="#">Cennik</a></li>
    <li><a href="#">FAQ</a></li>
    <li><a href="#">Opinie</a></li>
  </ul>
  <a href="#pricing" class="btn btn-primary">Kup Teraz</a>
</nav>

<section class="hero">
  <div class="badge">Wszystkie systemy sprawne</div>
  <h1>PANDORA</h1>
  <p>Najbezpieczniejszy i najbardziej zaawansowany klient do Minecraft</p>

  <div class="hero-buttons">
    <a href="#pricing" class="btn btn-primary">Kup Teraz</a>
    <a href="https://discord.gg/pdm4xuKr" target="_blank" class="btn btn-outline">Dowiedz się więcej</a>
  </div>

  <div class="hero-info">
    Dołącz do 10,000+ użytkowników • Minecraft 1.21.4 • Fabric
  </div>
</section>

<section id="pricing" class="pricing">
  <h2>Wybierz Swój Plan</h2>
  <p>Uczciwa cena za produkt klasy premium</p>

  <div class="cards">

    <div class="card">
      <div class="price">50 PLN / 30 dni</div>
      <ul class="features">
        <li>Pełny dostęp</li>
        <li>Wszystkie aktualizacje</li>
        <li>Wsparcie 24/7</li>
        <li>Nielimitowane zmiany HWID</li>
      </ul>
      <button class="btn btn-primary">Kup</button>
      <div class="payments">Stripe • BLIK • Przelew • Paysafecard</div>
    </div>

    <div class="card highlight">
      <div class="price">100 PLN / Na zawsze</div>
      <ul class="features">
        <li>Pełny dostęp</li>
        <li>Wszystkie aktualizacje</li>
        <li>Dostęp do bety</li>
        <li>Priorytetowe wsparcie</li>
        <li>Wsparcie 24/7</li>
        <li>Nielimitowane zmiany HWID</li>
      </ul>
      <button class="btn btn-primary">Kup</button>
      <div class="payments">Stripe • BLIK • Przelew • Paysafecard</div>
    </div>

    <div class="card">
      <div class="price">80 PLN / 90 dni</div>
      <ul class="features">
        <li>Pełny dostęp</li>
        <li>Wszystkie aktualizacje</li>
        <li>Wsparcie 24/7</li>
        <li>Nielimitowane zmiany HWID</li>
      </ul>
      <button class="btn btn-primary">Kup</button>
      <div class="payments">Stripe • BLIK • Przelew • Paysafecard</div>
    </div>

  </div>
</section>

<footer>
  © 2026 Pandora Client
</footer>

</body>
</html>

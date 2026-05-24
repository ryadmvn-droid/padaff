<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>PADAFF — Streetwear</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;700;900&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Inter',sans-serif;
    }

    body{
      background:#0a0a0a;
      color:white;
      overflow-x:hidden;
    }

    a{
      text-decoration:none;
      color:white;
    }

    header{
      position:fixed;
      top:0;
      left:0;
      width:100%;
      padding:20px 60px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      z-index:1000;
      background:rgba(0,0,0,0.5);
      backdrop-filter:blur(10px);
    }

    .logo{
      font-size:28px;
      font-weight:900;
      letter-spacing:6px;
    }

    nav{
      display:flex;
      gap:40px;
    }

    nav a{
      font-size:14px;
      text-transform:uppercase;
      transition:0.3s;
    }

    nav a:hover{
      opacity:0.5;
    }

    .hero{
      height:100vh;
      background:
      linear-gradient(rgba(0,0,0,0.5),rgba(0,0,0,0.7)),
      url('https://images.unsplash.com/photo-1523398002811-999ca8dec234?q=80&w=1600&auto=format&fit=crop');
      background-size:cover;
      background-position:center;
      display:flex;
      align-items:center;
      padding:0 8%;
    }

    .hero-content{
      max-width:650px;
    }

    .hero h1{
      font-size:90px;
      line-height:0.95;
      margin-bottom:20px;
      text-transform:uppercase;
    }

    .hero p{
      font-size:18px;
      color:#d0d0d0;
      margin-bottom:35px;
      line-height:1.6;
    }

    .btn{
      display:inline-block;
      padding:16px 38px;
      background:white;
      color:black;
      font-weight:700;
      border-radius:50px;
      transition:0.3s;
    }

    .btn:hover{
      transform:translateY(-3px);
      background:#d9d9d9;
    }

    .section{
      padding:120px 8%;
    }

    .section-title{
      font-size:48px;
      margin-bottom:60px;
      text-transform:uppercase;
      font-weight:900;
    }

    .products{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:30px;
    }

    .card{
      background:#111;
      border-radius:20px;
      overflow:hidden;
      transition:0.4s;
      cursor:pointer;
    }

    .card:hover{
      transform:translateY(-10px);
    }

    .card img{
      width:100%;
      height:420px;
      object-fit:cover;
    }

    .card-content{
      padding:20px;
    }

    .card h3{
      font-size:22px;
      margin-bottom:10px;
    }

    .price{
      color:#b3b3b3;
      font-size:16px;
    }

    .banner{
      height:70vh;
      border-radius:30px;
      background:
      linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.7)),
      url('https://images.unsplash.com/photo-1515886657613-9f3515b0c78f?q=80&w=1600&auto=format&fit=crop');
      background-size:cover;
      background-position:center;
      display:flex;
      align-items:center;
      padding:60px;
      margin-top:80px;
    }

    .banner h2{
      font-size:70px;
      max-width:700px;
      text-transform:uppercase;
      line-height:1;
    }

    footer{
      padding:60px 8%;
      border-top:1px solid #222;
      display:flex;
      justify-content:space-between;
      flex-wrap:wrap;
      gap:20px;
    }

    footer p{
      color:#999;
    }

    @media(max-width:900px){

      header{
        padding:20px;
      }

      nav{
        gap:20px;
      }

      .hero h1{
        font-size:58px;
      }

      .banner h2{
        font-size:42px;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="logo">PADAFF</div>

    <nav>
      <a href="#">Accueil</a>
      <a href="#">Shop</a>
      <a href="#">Collections</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-content">
      <h1>Neo Street Wear</h1>

      <p>
        PADAFF mélange l’univers streetwear futuriste,
        minimaliste et dark avec une identité inspirée
        des grandes marques premium.
      </p>

      <a href="#" class="btn">Découvrir la collection</a>
    </div>
  </section>

  <section class="section">

    <h2 class="section-title">Nouveautés</h2>

    <div class="products">

      <div class="card">
        <img src="https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?q=80&w=1200&auto=format&fit=crop" alt="">
        <div class="card-content">
          <h3>T-Shirt Shadow</h3>
          <div class="price">49€</div>
        </div>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1503341504253-dff4815485f1?q=80&w=1200&auto=format&fit=crop" alt="">
        <div class="card-content">
          <h3>Hoodie Eclipse</h3>
          <div class="price">89€</div>
        </div>
      </div>

      <div class="card">
        <img src="https://images.unsplash.com/photo-1529139574466-a303027c1d8b?q=80&w=1200&auto=format&fit=crop" alt="">
        <div class="card-content">
          <h3>Veste Gotham</h3>
          <div class="price">129€</div>
        </div>
      </div>

    </div>

    <div class="banner">
      <h2>
        Designed For The Underground
      </h2>
    </div>

  </section>

  <footer>
    <div class="logo">PADAFF</div>

    <p>
      © 2026 PADAFF — Tous droits réservés
    </p>
  </footer>

</body>
</html>

<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Blog des Lapins</title>

  <!-- Favicon -->
  <link rel="icon" href="https://github.com/Mv0178/tonlapin.com/blob/main/image-removebg-preview.png?raw=true" type="image/png">

  <style>
    /* Reset de base */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    /* Style général du body avec l'arrière-plan personnalisé */
    body {
      font-family: 'Arial', sans-serif;
      background-image: url('https://upload.wikimedia.org/wikipedia/commons/f/f5/Lapin_belier_hollandais.jpg');
      background-size: cover;
      background-position: center;
      color: #333;
      line-height: 1.6;
      padding-top: 80px; /* Pour que le contenu ne soit pas caché derrière le menu */
    }

    /* En-tête */
    header {
      background-color: rgba(255, 182, 193, 0.8); /* Fond légèrement transparent */
      color: white;
      text-align: center;
      padding: 20px 0;
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 10;
    }

    header .logo h1 {
      font-size: 2.5rem;
      color: #ff1493;
    }

    header nav {
      background-color: rgba(255, 105, 180, 0.8); /* Fond transparent pour la barre de menu */
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      padding: 10px 0;
      z-index: 9;
      display: flex;
      justify-content: center;
    }

    header nav ul {
      display: flex;
      justify-content: center;
    }

    header nav ul li {
      list-style: none;
      margin: 0 20px;
    }

    header nav ul li a {
      color: white;
      text-decoration: none;
      font-size: 1.2rem;
      padding: 10px 15px;
      border-radius: 5px;
      transition: background-color 0.3s ease;
    }

    header nav ul li a:hover {
      background-color: #ff1493;
    }

    /* Image dans la barre de recherche (icône) */
    header nav ul li a img {
      width: 30px;
      height: 30px;
      vertical-align: middle;
      margin-right: 8px;
    }

    /* Section Accueil avec des images défilantes */
    .carousel-container {
      position: relative;
      width: 100%;
      overflow: hidden;
      margin-top: 120px; /* Décalage pour que le carrousel ne soit pas caché */
      text-align: center; /* Centrer le contenu du carrousel */
    }

    .carousel {
      display: flex;
      justify-content: center; /* Centrer les images dans le carrousel */
      transition: transform 1s ease-in-out;
    }

    .carousel img {
      width: 80%; /* Ajuste la taille des images */
      max-width: 600px;
      height: auto;
      object-fit: cover;
      border-radius: 10px;
      margin: 0 10px; /* Espace entre les images */
    }

    /* Section des Articles */
    .section-header {
      text-align: center;
      color: #ff1493;
      font-size: 2.5rem;
      margin: 20px 0;
    }

    .article {
      display: flex;
      margin-bottom: 30px;
      align-items: center;
      padding: 20px;
      background-color: white;
      border-radius: 10px;
      box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    }

    .article img {
      width: 200px;
      height: 150px;
      margin-right: 20px;
      border-radius: 10px;
    }

    .article h3 {
      color: #ff1493;
    }

    .shop-link {
      display: inline-block;
      background-color: #ff1493;
      color: white;
      padding: 10px 20px;
      text-decoration: none;
      border-radius: 5px;
      margin-top: 10px;
    }

    .shop-link:hover {
      background-color: #ff69b4;
    }

    /* Footer */
    footer {
      background-color: rgba(255, 182, 193, 0.8);
      text-align: center;
      padding: 20px;
      color: white;
      margin-top: 40px;
    }

    /* Responsiveness */
    @media (max-width: 768px) {
      header .logo h1 {
        font-size: 2rem;
      }

      header nav ul {
        flex-direction: column;
      }

      header nav ul li {
        margin: 10px 0;
      }

      .article {
        flex-direction: column;
        align-items: flex-start;
      }

      .carousel img {
        height: 250px;
      }
    }
  </style>
</head>
<body>
  <!-- En-tête -->
  <header>
    <div class="logo">
      <h1>Bienvenue sur le Blog des Lapins</h1>
      <p>Tout ce que vous devez savoir sur les lapins, leurs soins et accessoires.</p>
    </div>
    <!-- Menu de navigation en haut -->
    <nav>
      <ul>
        <li><a href="#accueil"><img src="https://github.com/Mv0178/tonlapin.com/blob/main/image-removebg-preview.png?raw=true" alt="Lapin">Accueil</a></li>
        <li><a href="#articles">Articles</a></li>
        <li><a href="#tutos">Tutoriels</a></li>
        <li><a href="#shop">Boutique</a></li>
        <li><a href="#help">Aide</a></li>
      </ul>
    </nav>
  </header>

  <!-- Section Accueil avec des images défilantes -->
  <section id="accueil">
    <div class="carousel-container">
      <div class="carousel">
        <a href="#shop"><img src="https://github.com/Mv0178/tonlapin.com/blob/main/image-removebg-preview%20(2).png?raw=true" alt="Accessoires pour lapins"></a>
        <a href="#shop"><img src="https://cdn.webshopapp.com/shops/345024/files/452455068/laisser-un-lapin-en-liberte-dans-le-jardin-attenti.jpg" alt="Lapins en liberté"></a>
        <a href="#shop"><img src="https://github.com/Mv0178/tonlapin.com/blob/main/image-removebg-preview%20(3).png?raw=true" alt="Alimentation pour lapins"></a>        
      </div>
    </div>
  </section>

  <!-- Section Articles -->
  <section id="articles">
    <h2 class="section-header">Nos Derniers Articles</h2>
    <div class="article">
      <img src="https://www.zoomalia.com/blogz/228/l_clapier.jpg" alt="Lapin adorable">
      <div>
        <h3>Comment créer un enclos pour votre lapin</h3>
        <p>Un espace sécurisé pour votre lapin est essentiel pour sa santé et son bien-être. Découvrez comment construire un enclos confortable et sécurisé pour votre petit compagnon !</p>
        <a href="#articles" class="shop-link">Lire l'article complet</a>
      </div>
    </div>
  </section>

  <!-- Section Tutoriels -->
  <section id="tutos">
    <h2 class="section-header">Nos Tutoriels</h2>
    <div class="article">
      <img src="https://www.mouvement-metropole.fr/wp-content/uploads/2024/09/nettoyer-la-cage-de-votre-lapin-astuces-et-methodes-pour-un-habitat-impeccable_66d6c0d2c411e-scaled.jpg" alt="Soin du lapin">
      <div>
        <h3>Comment entretenir la cage de votre lapin</h3>
        <p>Un environnement propre et sain est crucial pour le bien-être de votre lapin. Apprenez à nettoyer et à entretenir la cage de votre compagnon à grandes oreilles.</p>
        <a href="#tutos" class="shop-link">Voir le tutoriel</a>
      </div>
    </div>
  </section>

  <!-- Section Boutique -->
  <section id="shop">
    <h2 class="section-header">Notre Boutique</h2>
    <p>Découvrez nos produits exclusifs pour prendre soin de votre lapin et lui offrir le meilleur !</p>

    <div class="article">
      <img src="https://static.zoomalia.com/prod_img/143835/xl_3433ad7c2ebb96fcba7cda0cf54a2e802f51699974267.jpg" alt="Panier pour lapin">
      <div>
        <h3>Panier Douillet pour Lapin</h3>
        <p>Un panier confortable et doux pour que votre lapin se sente à l'aise à tout moment.</p>
      </div>
      <div class="product-price">€19,99</div>
      <button onclick="alert('Produit ajouté au panier!')">Ajouter au panier</button>
    </div>

    <div class="article">
      <img src="https://m.media-amazon.com/images/I/71B-SbgU54L.jpg" alt="Accessoires pour lapin">
      <div>
        <h3>Accessoires pour Lapin</h3>
        <p>Accessoires essentiels pour le confort et la sécurité de votre compagnon à grandes oreilles.</p>
      </div>
      <div class="product-price">€9,99</div>
      <button onclick="alert('Produit ajouté au panier!')">Ajouter au panier</button>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2024 Blog des Lapins. Tous droits réservés.</p>
  </footer>
</body>
</html>

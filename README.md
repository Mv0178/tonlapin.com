<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Blog des Lapins</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f8ff;
      display: flex;
    }
    header {
      background-color: #ffb6c1;
      color: #fff;
      text-align: center;
      padding: 20px;
      width: 100%;
    }
    header h1 {
      margin: 0;
    }
    nav {
      background-color: #ff69b4;
      color: white;
      width: 200px;
      padding-top: 20px;
      position: fixed;
      top: 0;
      left: 0;
      height: 100%;
      box-shadow: 2px 0px 5px rgba(0, 0, 0, 0.1);
    }
    nav a {
      color: white;
      text-decoration: none;
      padding: 10px;
      display: block;
      border-bottom: 1px solid #fff;
      transition: background-color 0.3s;
    }
    nav a:hover {
      background-color: #ff1493;
    }
    .menu-item {
      padding-left: 20px;
      display: none;
    }
    nav .submenu:hover .menu-item {
      display: block;
    }
    main {
      margin-left: 220px;
      padding: 20px;
      width: 100%;
    }
    section {
      padding: 20px;
      margin: 20px;
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    }
    .section-header {
      color: #ff1493;
      font-size: 2em;
    }
    .article, .product {
      display: flex;
      margin-bottom: 20px;
      align-items: center;
    }
    .article img, .product img {
      width: 200px;
      height: 150px;
      margin-right: 20px;
      border-radius: 10px;
    }
    .article div, .product div {
      max-width: 600px;
    }
    .article h3, .product h4 {
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
    .product-price {
      font-weight: bold;
      color: #ff1493;
    }
    footer {
      background-color: #ffb6c1;
      text-align: center;
      padding: 20px;
      color: white;
      margin-top: 20px;
    }
    .carousel img {
      width: 100%;
      height: 300px;
      object-fit: cover;
      border-radius: 10px;
    }
    .carousel {
      display: flex;
      overflow-x: auto;
      gap: 10px;
    }
  </style>
</head>
<body>

  <!-- Navigation latérale -->
  <nav>
    <a href="#accueil">Accueil</a>
    <a href="#articles">Articles</a>
    <a href="#tutos">Tutoriels</a>
    <a href="#shop">Boutique</a>
    <a href="#help">Aide</a>

    <div class="submenu">
      <a href="#">Menu Déroulant</a>
      <div class="menu-item">
        <a href="#">Sous-Menu 1</a>
        <a href="#">Sous-Menu 2</a>
      </div>
    </div>
  </nav>

  <main>
    <!-- Section Accueil avec des images -->
    <header>
      <h1>Bienvenue sur le Blog des Lapins</h1>
      <p>Tout ce que vous devez savoir sur les lapins, leurs soins et accessoires.</p>
    </header>

    <section id="accueil">
      <div class="carousel">
        <img src="https://via.placeholder.com/1200x300?text=Lapins+en+liberté" alt="Lapins en liberté">
        <img src="https://via.placeholder.com/1200x300?text=Accessoires+pour+lapins" alt="Accessoires pour lapins">
        <img src="https://via.placeholder.com/1200x300?text=Alimentation+pour+lapins" alt="Alimentation pour lapins">
      </div>
    </section>

    <!-- Section Articles -->
    <section id="articles">
      <h2 class="section-header">Nos Derniers Articles</h2>
      
      <div class="article">
        <img src="https://via.placeholder.com/200x150" alt="Lapin adorable">
        <div>
          <h3>Comment créer un enclos pour votre lapin</h3>
          <p>Un espace sécurisé pour votre lapin est essentiel pour sa santé et son bien-être. Découvrez comment construire un enclos confortable et sécurisé pour votre petit compagnon !</p>
          <a href="#" class="shop-link">Lire l'article complet</a>
        </div>
      </div>

      <div class="article">
        <img src="https://via.placeholder.com/200x150" alt="Lapin joyeux">
        <div>
          <h3>Les meilleurs aliments pour votre lapin</h3>
          <p>Les lapins ont des besoins alimentaires spécifiques. Dans cet article, nous vous guidons pour choisir les meilleures nourritures et friandises pour votre ami à grandes oreilles.</p>
          <a href="#" class="shop-link">Lire l'article complet</a>
        </div>
      </div>

      <!-- Plus d'articles peuvent être ajoutés ici -->
    </section>

    <!-- Section Tutoriels -->
    <section id="tutos">
      <h2 class="section-header">Nos Tutoriels</h2>

      <div class="article">
        <img src="https://via.placeholder.com/200x150" alt="Soin du lapin">
        <div>
          <h3>Comment entretenir la cage de votre lapin</h3>
          <p>Un environnement propre et sain est crucial pour le bien-être de votre lapin. Apprenez à nettoyer et à entretenir la cage de votre compagnon à grandes oreilles.</p>
          <a href="#" class="shop-link">Voir le tutoriel</a>
        </div>
      </div>

      <div class="article">
        <img src="https://via.placeholder.com/200x150" alt="Lapin curieux">
        <div>
          <h3>Éviter les maladies courantes chez les lapins</h3>
          <p>Les lapins peuvent être sujets à diverses maladies. Découvrez les symptômes à surveiller et comment prévenir les problèmes de santé fréquents chez les lapins.</p>
          <a href="#" class="shop-link">Voir le tutoriel</a>
        </div>
      </div>
      
      <!-- Ajoutez plus de tutoriels ici -->
    </section>

    <!-- Section Boutique -->
    <section id="shop">
      <h2 class="section-header">Notre Boutique</h2>
      <p>Découvrez nos produits exclusifs pour prendre soin de votre lapin et lui offrir le meilleur !</p>

      <div class="product">
        <img src="https://via.placeholder.com/100" alt="Panier pour lapin">
        <div>
          <h4>Panier Douillet pour Lapin</h4>
          <p>Un panier confortable et doux pour que votre lapin se sente à l'aise à tout moment.</p>
        </div>
        <div class="product-price">€19,99</div>
        <button onclick="alert('Produit ajouté au panier!')">Ajouter au panier</button>
      </div>

      <div class="product">
        <img src="https://via.placeholder.com/100" alt="Cage pour lapin">
        <div>
          <h4>Cage Spacieuse pour Lapin</h4>
          <p>Une cage spacieuse et sécurisée pour permettre à votre lapin de vivre confortablement.</p>
        </div>
        <div class="product-price">€49,99</div>
        <button onclick="alert('Produit ajouté au panier!')">Ajouter au panier</button>
      </div>

      <!-- Plus de produits peuvent être ajoutés ici -->
    </section>

    <!-- Section Aide -->
    <section id="help">
      <h2 class="section-header">Aide pour les propriétaires de lapins</h2>

      <div class="article">
        <h3>Comment savoir si mon lapin est malade ?</h3>
        <p>Observez des signes comme un appétit diminué, de la léthargie ou des changements dans le pelage. Il est important de consulter un vétérinaire en cas de doute.</p>
      </div>

      <div class="article">
        <h3>Quelle nourriture donner à mon lapin ?</h3>
        <p>Les lapins ont besoin d'un régime riche en foin, légumes frais et un accès limité aux fruits et granulés.</p>
      </div>

      <!-- Ajoutez plus d'articles d'aide -->
    </section>

  </main>

  <footer>
    <p>© 2024 Blog des Lapins | Tous droits réservés</p>
  </footer>

  <script>
    // Si vous avez besoin de personnaliser davantage le comportement du panier
    const addToCartButtons = document.querySelectorAll('button');
    addToCartButtons.forEach(button => {
      button.addEventListener('click', () => {
        alert('Produit ajouté au panier!');
      });
    });
  </script>

</body>
</html>

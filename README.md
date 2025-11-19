<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ovencia — Beauté naturelle</title>

  <style>
    body {
      font-family: system-ui, sans-serif;
      margin: 0;
      padding: 0;
      background: #fff;
      color: #222;
      line-height: 1.6;
    }

    main {
      padding: 40px;
      max-width: 1200px;
      margin: auto;
    }

    .hero {
      display: flex;
      justify-content: space-between;
      gap: 40px;
      flex-wrap: wrap;
      padding-bottom: 60px;
      border-bottom: 1px solid #eee;
    }

    .eyebrow {
      text-transform: uppercase;
      font-size: 12px;
      color: #888;
      margin-bottom: 8px;
      font-weight: 600;
    }

    h1 {
      font-size: 42px;
      margin: 0;
    }

    .lead {
      font-size: 18px;
      color: #444;
      max-width: 500px;
    }

    .buttons {
      margin-top: 20px;
      display: flex;
      gap: 14px;
    }

    .btn {
      padding: 10px 18px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 600;
      border: none;
    }

    .btn.primary {
      background: #333;
      color: white;
    }

    .btn.ghost {
      background: transparent;
      border: 2px solid #ccc;
      color: #333;
    }

    aside .card {
      border: 1px solid #eee;
      padding: 20px;
      border-radius: 14px;
      width: 300px;
      background: #fafafa;
    }

    .product-image {
      background: #eaeaea;
      height: 160px;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 14px;
      color: #777;
      margin-bottom: 14px;
    }

    .product-title {
      font-weight: 700;
      font-size: 18px;
    }

    .product-sub {
      color: #666;
      margin-bottom: 10px;
    }

    .pill {
      background: #eee;
      padding: 4px 10px;
      border-radius: 20px;
      font-size: 12px;
      font-weight: 600;
    }

    /* Grid Produits */
    .grid-3 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .card {
      background: white;
      border-radius: 12px;
      padding: 20px;
      border: 1px solid #eee;
    }

    /* Contact */
    .contact-grid {
      display: flex;
      gap: 40px;
      flex-wrap: wrap;
      margin-top: 20px;
    }

    form.card {
      width: 320px;
      display: flex;
      flex-direction: column;
      gap: 12px;
    }

    input, textarea {
      padding: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-size: 15px;
      width: 100%;
    }

    textarea {
      min-height: 120px;
    }

    footer {
      margin-top: 60px;
      padding: 30px;
      text-align: center;
      color: #666;
      font-size: 14px;
      border-top: 1px solid #eee;
    }

  </style>
</head>

<body>

<main>

  <!-- HERO -->
  <section class="hero">
    <div>
      <div class="eyebrow">Soin naturel & innovant</div>
      <h1>La beauté née de la coquille d'œuf</h1>

      <p class="lead">
        Ovencia transforme la coquille d'œuf en actif cosmétique régénérant.
        Des soins 100% naturels, efficaces et respectueux de la peau et de la planète.
      </p>

      <div class="buttons">
        <a class="btn primary" href="#produits">Découvrir nos soins</a>
        <a class="btn ghost" href="#philosophie">Notre démarche</a>
      </div>

      <div style="margin-top:20px;font-size:14px;color:#777">
        Fabriqué en Europe · Ingrédients naturels · Zéro déchet
      </div>
    </div>

    <aside>
      <div class="card">
        <div class="product-image">Photo produit (remplacer)</div>
        <div class="product-title">Crème Régénérante Ovencia — 50 ml</div>
        <div class="product-sub">Coquille d'œuf · Beurre de karité · Gel d'aloe</div>

        <div style="display:flex;gap:8px;margin-top:12px;align-items:center">
          <span class="pill">100% naturel</span>
          <span style="color:#999;font-weight:600">·</span>
          <div style="color:#777">Texture riche, absorption rapide</div>
        </div>

        <div style="margin-top:14px;display:flex;gap:10px">
          <a class="btn primary" href="#contact">Demande d'échantillon</a>
          <a class="btn" style="background:transparent;border:2px solid #ddd;color:#333" href="#produits">Voir la fiche</a>
        </div>
      </div>
    </aside>
  </section>

  <!-- PHILOSOPHIE -->
  <section id="philosophie">
    <h2>Notre philosophie</h2>

    <p style="color:#666;max-width:600px">
      Chez Ovencia, la coquille d'œuf symbolise la pureté et la régénération.
      Nous valorisons ce trésor naturel en le transformant en ingrédient actif
      pour des soins efficaces, sûrs et durables.
    </p>

    <ul style="margin-top:12px;color:#777">
      <li>Ingrédients 100% naturels</li>
      <li>Formules artisanales et transparentes</li>
      <li>Emballages recyclables en verre</li>
    </ul>
  </section>

  <!-- PRODUITS -->
  <section id="produits">
    <h2>Nos produits</h2>

    <div class="grid-3">

      <div class="card">
        <div class="product-image">Crème Régénérante — 50 ml</div>
        <h3>Régénération</h3>
        <p class="product-sub">Coquille d'œuf · Karité · Lavande</p>
        <p class="muted">Hydrate, apaise et aide à la régénération cutanée.</p>
      </div>

      <div class="card">
        <div class="product-image">Crème Lissante — 50 ml</div>
        <h3>Lissage</h3>
        <p class="product-sub">Coquille micronisée · Amande douce · Aloe</p>
        <p class="muted">Texture légère, idéale pour peaux sensibles.</p>
      </div>

      <div class="card">
        <div class="product-image">Baume Nourrissant — 30 ml</div>
        <h3>Nourrissant</h3>
        <p class="product-sub">Coquille · Cire d'abeille · Miel</p>
        <p class="muted">Idéal pour les zones sèches et abîmées.</p>
      </div>

    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Contact & partenariats</h2>

    <div class="contact-grid">

      <!-- FORM -->
      <form class="card" method="POST" action="mailto:contact@ovencia.be" enctype="text/plain">
        <label for="name">Nom</label>
        <input id="name" name="name" required>

        <label for="email">Email</label>
        <input id="email" name="email" type="email" required>

        <label for="message">Message</label>
        <textarea id="message" name="message" required></textarea>

        <button class="btn primary" type="submit">Envoyer</button>

        <p class="small" style="font-size:13px;margin-top:4px;color:#666">
          Ou écris-nous : <a href="mailto:contact@ovencia.be">contact@ovencia.be</a>
        </p>
      </form>

      <!-- INFO -->
      <div style="flex:1;min-width:260px">
        <div class="card" style="background:#fafafa">
          <h4>Informations</h4>
          <p class="muted">
            Pour toute demande d'échantillons, distribution ou partenariat,
            contacte-nous — nous te répondrons rapidement.
          </p>

          <ul style="color:#777">
            <li>Fabrication : Europe</li>
            <li>Production : artisanale</li>
            <li>Emballages : verre & carton recyclable</li>
          </ul>
        </div>
      </div>

    </div>
  </section>

</main>

<footer>
  © <span id="year"></span> Ovencia — Tous droits réservés · Beauté naturelle
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>

</body>
</html>

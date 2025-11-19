<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ovencia — Beauté naturelle</title>

  <!-- STYLES -->
  <style>
    :root {
      --muted: #666;
      --eggshell: #f6f3e9;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: "Inter", Arial, sans-serif;
      color: #222;
      line-height: 1.6;
    }

    main {
      max-width: 1100px;
      margin: auto;
      padding: 20px;
    }

    h1, h2, h4 {
      margin: 0 0 10px;
    }

    /* HERO */
    .hero {
      display: flex;
      gap: 40px;
      flex-wrap: wrap;
      align-items: center;
      margin-bottom: 50px;
    }

    .eyebrow {
      font-size: 14px;
      color: var(--muted);
      margin-bottom: 8px;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.5px;
    }

    .lead {
      font-size: 1.1rem;
      color: #444;
      max-width: 500px;
    }

    .buttons {
      display: flex;
      gap: 10px;
      margin-top: 12px;
    }

    .btn, button.btn {
      padding: 10px 18px;
      border-radius: 8px;
      font-weight: 600;
      text-decoration: none;
      display: inline-block;
      border: none;
      cursor: pointer;
      font-family: inherit;
      font-size: 14px;
      transition: all 0.2s;
    }
    .btn.primary, button.btn.primary {
      background: #222;
      color: white;
    }
    .btn.primary:hover, button.btn.primary:hover {
      background: #000;
    }
    .btn.ghost {
      border: 2px solid #222;
      color: #222;
      background: transparent;
    }
    .btn.ghost:hover {
      background: #222;
      color: white;
    }

    .pill {
      padding: 4px 10px;
      background: var(--eggshell);
      border-radius: 999px;
      font-size: 12px;
      font-weight: bold;
    }

    .card {
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.06);
    }

    .product-image {
      height: 150px;
      background: #eee;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 10px;
      margin-bottom: 12px;
      color: #777;
      font-size: 14px;
    }

    .product-title {
      font-weight: 600;
      font-size: 18px;
      margin-bottom: 4px;
    }

    .product-sub {
      font-size: 14px;
      color: var(--muted);
      margin-bottom: 8px;
    }

    .grid-3 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 20px;
      margin-top: 20px;
    }

    .muted { 
      color: var(--muted); 
    }

    .feature {
      margin-bottom: 16px;
    }

    .feature h4 {
      margin-bottom: 6px;
    }

    /* CONTACT */
    .contact-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 20px;
    }

    .contact-grid > * {
      flex: 1;
      min-width: 300px;
    }

    input, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 4px;
      margin-bottom: 12px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 14px;
      font-family: inherit;
    }
    
    input:focus, textarea:focus {
      outline: none;
      border-color: #222;
    }
    
    textarea { 
      min-height: 120px;
      resize: vertical;
    }

    label {
      display: block;
      font-weight: 600;
      font-size: 14px;
      margin-top: 8px;
    }

    footer {
      text-align: center;
      padding: 30px 0;
      color: #777;
      margin-top: 40px;
      border-top: 1px solid #eee;
    }

    section {
      margin-bottom: 60px;
    }
  </style>

  <script>
    function handleForm(e) {
      e.preventDefault();
      alert("Message envoyé !");
      e.target.reset();
      return false;
    }

    window.onload = () => {
      document.getElementById("year").textContent = new Date().getFullYear();
    };
  </script>
</head>

<body>

<main>

  <!-- HERO -->
  <section class="hero">
    <div>
      <div class="eyebrow">Soin naturel & innovant</div>
      <h1>La beauté née de la coquille d'œuf</h1>
      <p class="lead">Ovencia transforme la coquille d'œuf en actif cosmétique régénérant. Des soins 100% naturels, efficaces et respectueux de la peau et de la planète.</p>

      <div class="buttons">
        <a class="btn primary" href="#produits">Découvrir nos soins</a>
        <a class="btn ghost" href="#philosophie">Notre démarche</a>
      </div>

      <div style="margin-top:20px;font-size:14px;color:var(--muted)">
        Fabriqué en Europe · Ingrédients naturels · Zéro déchet
      </div>
    </div>

    <aside>
      <div class="card">
        <div class="product-image">Photo produit (remplacer)</div>
        <div class="product-title">Crème Régénérante Ovencia — 50 ml</div>
        <div class="product-sub">Poudre de coquille d'œuf · Beurre de karité · Gel d'aloe</div>

        <div style="display:flex;gap:8px;margin-top:12px;align-items:center;flex-wrap:wrap">
          <span class="pill">100% naturel</span>
          <span style="color:var(--muted);font-weight:600">·</span>
          <div class="muted">Texture riche, absorption rapide</div>
        </div>

        <div style="margin-top:14px;display:flex;gap:10px;flex-wrap:wrap">
          <a class="btn primary" href="#contact">Demande d'échantillon</a>
          <a class="btn" style="border:2px solid #ddd;color:#333" href="#produits">Voir la fiche</a>
        </div>
      </div>
    </aside>
  </section>

  <!-- PHILOSOPHIE -->
  <section id="philosophie">
    <h2>Notre philosophie</h2>

    <div style="display:flex;gap:30px;flex-wrap:wrap;align-items:flex-start;margin-top:20px">
      <div style="flex:1;min-width:300px">
        <p class="muted">
          Chez Ovencia, la coquille d'œuf symbolise la pureté et la régénération.
          Nous valorisons ce trésor naturel en le transformant en ingrédient actif,
          pour des soins efficaces, sûrs et durables.
        </p>

        <ul class="muted">
          <li>Ingrédients 100% naturels</li>
          <li>Formules artisanales et transparentes</li>
          <li>Emballages recyclables en verre</li>
        </ul>
      </div>

      <div style="width:300px">
        <div class="feature">
          <h4>Procédé purifié</h4>
          <p class="muted">La coquille est stérilisée et micronisée pour préserver sa richesse minérale.</p>
        </div>

        <div class="feature">
          <h4>Écoresponsable</h4>
          <p class="muted">Nous valorisons un sous-produit naturel pour une beauté durable.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- PRODUITS -->
  <section id="produits">
    <h2>Nos produits</h2>

    <div class="grid-3">

      <div class="card">
        <div class="product-image">Crème Régénérante — 50 ml</div>
        <div class="product-title">Régénération</div>
        <div class="product-sub">Coquille d'œuf, karité, lavande</div>
        <p class="muted">Hydrate, apaise et régénère la peau.</p>
      </div>

      <div class="card">
        <div class="product-image">Crème Lissante — 50 ml</div>
        <div class="product-title">Lissage</div>
        <div class="product-sub">Coquille, amande douce, aloe</div>
        <p class="muted">Texture légère, idéale pour peaux sensibles.</p>
      </div>

      <div class="card">
        <div class="product-image">Baume Nourrissant — 30 ml</div>
        <div class="product-title">Nourrissant</div>
        <div class="product-sub">Coquille, cire d'abeille, miel</div>
        <p class="muted">Parfait pour zones sèches et abîmées.</p>
      </div>

    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Contact & partenariats</h2>

    <div class="contact-grid">

      <form class="card" onsubmit="return handleForm(event)">
        <label for="name">Nom</label>
        <input id="name" name="name" required>

        <label for="email">Email</label>
        <input id="email" name="email" type="email" required>

        <label for="message">Message</label>
        <textarea id="message" name="message" required></textarea>

        <button class="btn primary" type="submit">Envoyer</button>
      </form>

      <div class="card" style="background:linear-gradient(180deg,var(--eggshell),#fff)">
        <h4>Informations</h4>
        <p class="muted">Demandes d'échantillons, distribution, partenariats.</p>
        <ul class="muted">
          <li>Fabrication : Europe</li>
          <li>Production artisanale</li>
          <li>Emballages recyclables</li>
        </ul>
      </div>

    </div>
  </section>

</main>

<footer>
  © <span id="year"></span> Ovencia — Tous droits réservés
</footer>

</body>
</html>

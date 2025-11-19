<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ovencia — Beauté naturelle</title>

  <style>
    :root {
      --muted: #777;
      --eggshell: #f6f3e8;
    }
    body {
      font-family: sans-serif;
      margin: 0;
      background: #111;
      color: #fff;
      line-height: 1.6;
      padding: 40px;
    }
    h1, h2, h3, h4 { margin: 0 0 10px; }
    .lead { font-size: 18px; color: #ccc; }
    .muted { color: var(--muted); }
    .btn {
      padding: 10px 16px;
      border-radius: 8px;
      text-decoration: none;
      display: inline-block;
      font-weight: 600;
      transition: 0.2s;
    }
    .btn.primary {
      background: #fff;
      color: #111;
    }
    .btn.ghost {
      border: 2px solid #fff;
      color: #fff;
    }
    .hero {
      display: flex;
      gap: 40px;
      flex-wrap: wrap;
    }
    .card {
      background: #1a1a1a;
      padding: 18px;
      border-radius: 12px;
    }
    .product-image {
      background: #333;
      padding: 40px;
      border-radius: 12px;
      text-align: center;
      margin-bottom: 10px;
    }
    .contact-grid {
      display: flex;
      gap: 30px;
      flex-wrap: wrap;
      align-items: flex-start;
    }
    form.card input,
    form.card textarea {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      margin-bottom: 12px;
      border: 1px solid #333;
      background: #000;
      color: #fff;
    }
    textarea { min-height: 120px; }
    footer {
      margin-top: 40px;
      text-align: center;
      color: #777;
    }
  </style>

  <script>
    function handleForm(event) {
      alert("Message envoyé !");
      event.preventDefault();
      return false;
    }
  </script>
</head>

<body>

<main>

  <!-- HERO -->
  <section class="hero">
    <div>
      <div class="eyebrow muted">Soin naturel & innovant</div>
      <h1>La beauté née de la coquille d'œuf</h1>
      <p class="lead">
        Ovencia transforme la coquille d'œuf en actif cosmétique régénérant.
        Des soins 100% naturels, efficaces et respectueux de la peau et de la planète.
      </p>

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
        <div class="product-image">Photo produit</div>
        <div class="product-title">Crème Régénérante Ovencia — 50 ml</div>
        <div class="product-sub muted">
          Poudre de coquille d'œuf · Beurre de karité · Gel d'aloe
        </div>

        <div style="display:flex;gap:8px;margin-top:12px;align-items:center">
          <span class="pill">100% naturel</span>
          <span class="muted">·</span>
          <div class="muted">Texture riche, absorption rapide</div>
        </div>

        <div style="margin-top:14px;display:flex;gap:10px">
          <a class="btn primary" href="#contact">Demande d'échantillon</a>
          <a class="btn" style="background:transparent;border:2px solid #ddd;color:#fff"
             href="#produits">Voir la fiche</a>
        </div>
      </div>
    </aside>
  </section>

  <!-- PHILOSOPHIE -->
  <section id="philosophie" style="margin-top:60px">
    <div style="display:flex;align-items:flex-start;gap:30px;flex-wrap:wrap">
      <div style="flex:1;min-width:300px">
        <h2>Notre philosophie</h2>
        <p class="muted">
          Chez Ovencia, la coquille d'œuf symbolise la pureté et la régénération.
          Nous valorisons ce trésor naturel en le transformant en ingrédient actif.
        </p>

        <ul class="muted">
          <li>Ingrédients 100% naturels</li>
          <li>Formules artisanales et transparentes</li>
          <li>Emballages recyclables en verre</li>
        </ul>
      </div>

      <div style="width:320px">
        <div class="card">
          <h4>Procédé purifié</h4>
          <div class="muted">
            La coquille est stérilisée et micronisée pour préserver sa richesse minérale.
          </div>
        </div>

        <div class="card" style="margin-top:12px">
          <h4>Écoresponsable</h4>
          <div class="muted">
            Nos soins valorisent un sous-produit naturel pour une beauté durable.
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- PRODUITS -->
  <section id="produits" style="margin-top:60px">
    <h2>Nos produits</h2>

    <div style="display:flex;gap:20px;flex-wrap:wrap">
      <div class="card" style="flex:1;min-width:260px">
        <div class="product-image">Crème Régénérante — 50 ml</div>
        <div class="product-title">Régénération</div>
        <div class="product-sub muted">Coquille d'œuf, karité, lavande</div>
        <div class="muted" style="margin-top:8px">
          Hydrate, apaise et aide à la régénération cutanée.
        </div>
      </div>

      <div class="card" style="flex:1;min-width:260px">
        <div class="product-image">Crème Lissante — 50 ml</div>
        <div class="product-title">Lissage</div>
        <div class="product-sub muted">Coquille micronisée, amande douce, aloe</div>
        <div class="muted" style="margin-top:8px">
          Texture légère, idéale pour peaux sensibles.
        </div>
      </div>

      <div class="card" style="flex:1;min-width:260px">
        <div class="product-image">Baume Nourrissant — 30 ml</div>
        <div class="product-title">Nourrissant</div>
        <div class="product-sub muted">Coquille, cire d'abeille, miel</div>
        <div class="muted" style="margin-top:8px">
          Idéal pour les zones sèches et abîmées.
        </div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" style="margin-top:60px">
    <h2>Contact & partenariats</h2>

    <div class="contact-grid">

      <!-- FORMULAIRE -->
      <form class="card" onsubmit="return handleForm(event)">
        <label for="name">Nom</label>
        <input id="name" name="name" placeholder="Votre nom" required>

        <label for="email">Email</label>
        <input id="email" name="email" type="email" placeholder="Votre email" required>

        <label for="message">Message</label>
        <textarea id="message" name="message" placeholder="Votre message…" required></textarea>

        <button class="btn primary" type="submit">Envoyer</button>

        <p class="muted" style="margin-top:12px;font-size:14px">
          Ou écris-nous directement :
          <a href="mailto:contact@ovencia.example">contact@ovencia.example</a>
        </p>
      </form>

      <!-- INFO -->
      <div class="card" style="background:linear-gradient(180deg,var(--eggshell),#fff);color:#000;">
        <h4>Informations</h4>
        <p>
          Pour toute demande d'échantillons, distribution ou partenariat, contacte-nous.
        </p>

        <ul>
          <li>Fabrication : Europe</li>
          <li>Production : artisanale, en petite série</li>
          <li>Emballages : verre et carton recyclable</li>
        </ul>
      </div>

    </div>
  </section>

</main>

<footer>
  © <span id="year"></span> Ovencia — Beauté naturelle
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>

</body>
</html>

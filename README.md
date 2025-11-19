<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ovencia — Beauté naturelle</title>

  <style>
    :root {
      --muted: #666;
      --eggshell: #f6f3e9;
    }

    body {
      margin: 0;
      font-family: Arial, sans-serif;
      color: #222;
      background: #fff;
      line-height: 1.6;
    }

    header, footer, main, section {
      padding: 20px;
      max-width: 1100px;
      margin: auto;
    }

    .hero {
      display: flex;
      gap: 40px;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
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

    .btn {
      padding: 10px 18px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 600;
      display: inline-block;
    }

    .btn.primary {
      background: #222;
      color: #fff;
    }

    .btn.ghost {
      background: transparent;
      border: 2px solid #222;
      color: #222;
    }

    .pill {
      padding: 4px 10px;
      border-radius: 999px;
      background: var(--eggshell);
      font-size: 12px;
      font-weight: bold;
    }

    .card {
      padding: 20px;
      border-radius: 12px;
      background: #fff;
      box-shadow: 0 6px 20px rgba(0,0,0,0.06);
    }

    .product-image {
      width: 100%;
      height: 160px;
      background: #eee;
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 10px;
      margin-bottom: 12px;
      color: #777;
      font-size: 14px;
    }

    .grid-3 {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 20px;
      margin-top: 14px;
    }

    .muted { color: var(--muted); }

    .contact-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }

    label {
      margin-top: 10px;
      display: block;
      font-size: 14px;
    }

    input, textarea {
      width: 100%;
      padding: 8px;
      border-radius: 6px;
      border: 1px solid #ccc;
      margin-top: 4px;
      box-sizing: border-box;
    }

    textarea {
      min-height: 110px;
    }

    footer {
      text-align: center;
      margin-top: 40px;
      padding: 40px 0;
      color: #777;
    }
  </style>

  <script>
    function handleForm(e) {
      alert("Message envoyé !");
      return true;
    }

    document.addEventListener("DOMContentLoaded", () => {
      document.getElementById("year").textContent = new Date().getFullYear();
    });
  </script>
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

      <div style="margin-top:20px;font-size:14px;color:var(--muted)">
        Fabriqué en Europe · Ingrédients naturels · Zéro déchet
      </div>
    </div>

    <aside>
      <div class="card">
        <div class="product-image">Image produit</div>
        <div class="product-title">Crème Régénérante — 50 ml</div>
        <div class="product-sub">Coquille d'œuf · Karité · Gel d'aloe</div>

        <div style="display:flex;gap:8px;margin-top:12px;align-items:center">
          <span class="pill">100% naturel</span>
          <span style="color:var(--muted);font-weight:600">·</span>
          <div class="muted">Texture riche, absorption rapide</div>
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
    <p class="muted">
      Chez Ovencia, la coquille d'œuf symbolise la pureté et la régénération.
      Nous valorisons ce trésor naturel en le transformant en ingrédient actif,
      pour des soins efficaces, sûrs et durables.
    </p>
  </section>

  <!-- PRODUITS -->
  <section id="produits">
    <h2>Nos produits</h2>

    <div class="grid-3">

      <div class="card">
        <div class="product-image">Crème Régénérante — 50 ml</div>
        <div class="product-title">Régénération</div>
        <div class="product-sub">Coquille d'œuf, karité, lavande</div>
        <div class="muted" style="margin-top:8px">
          Hydrate, apaise et aide la régénération cutanée.
        </div>
      </div>

      <div class="card">
        <div class="product-image">Crème Lissante — 50 ml</div>
        <div class="product-title">Lissage</div>
        <div class="product-sub">Amande douce, aloe</div>
        <div class="muted" style="margin-top:8px">
          Texture légère pour peaux sensibles.
        </div>
      </div>

      <div class="card">
        <div class="product-image">Baume Nourrissant — 30 ml</div>
        <div class="product-title">Nourrissant</div>
        <div class="product-sub">Coquille, cire d'abeille, miel</div>
        <div class="muted" style="margin-top:8px">
          Parfait pour zones sèches et abîmées.
        </div>
      </div>

    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact">
    <h2>Contact & partenariats</h2>

    <div class="contact-grid">

      <!-- FORMULAIRE -->
      <form class="card" method="POST" onsubmit="return handleForm(event)">

        <label for="name">Nom</label>
        <input id="name" name="name" type="text" placeholder="Ton nom" required>

        <label for="email">Email</label>
        <input id="email" name="email" type="email" placeholder="adresse@mail.com" required>

        <label for="message">Message</label>
        <textarea id="message" name="message" placeholder="Votre message..." required></textarea>

        <div style="margin-top:12px;display:flex;gap:4px;align-items:center">
          <button class="btn primary" type="submit">Envoyer</button>
        </div>

      </form>

      <!-- INFO -->
      <div style="padding:18px">
        <div class="card" style="background:linear-gradient(180deg,var(--eggshell),#fff)">
          <h4>Informations</h4>
          <p class="muted">
            Pour toute demande d'échantillons, distribution ou partenariat,
            contacte-nous — nous répondons rapidement.
          </p>

          <ul class="muted">
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
  © <span id="year"></span> Ovencia — Beauté naturelle
</footer>

</body>
</html>

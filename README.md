<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Agro Forte - Um Futuro Melhor</title>

  <style>
    /* ================= RESET ================= */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
      scroll-behavior: smooth;
    }

    body {
      background: #f4efe7;
      color: #3d2412;
      line-height: 1.7;
      overflow-x: hidden;
    }

    /* ================= ENTRADA ================= */
    #entrada {
      position: fixed;
      width: 100%;
      height: 100vh;
      background: linear-gradient(135deg,#3e2723,#5d4037,#8d6e63);
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      color: white;
      text-align: center;
      z-index: 9999;
      padding: 20px;
    }

    #entrada h1 { font-size: 3rem; }
    #entrada button {
      margin-top: 20px;
      padding: 15px 25px;
      border: none;
      border-radius: 10px;
      font-weight: bold;
      cursor: pointer;
    }

    /* ================= HEADER ================= */
    header {
      background: linear-gradient(rgba(0,0,0,0.6),rgba(0,0,0,0.6)),
      url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=1600&q=80');
      background-size: cover;
      background-position: center;
      color: white;
      text-align: center;
      padding: 120px 20px;
    }

    header h1 {
      font-size: 4rem;
      animation: piscar 3s infinite;
    }

    /* ================= MENU ================= */
    nav {
      background: #4e342e;
      position: sticky;
      top: 0;
      text-align: center;
      padding: 15px;
      z-index: 1000;
    }

    nav a {
      color: white;
      margin: 0 12px;
      text-decoration: none;
      font-weight: bold;
    }

    /* ================= SEÇÕES ================= */
    section {
      padding: 70px 10%;
    }

    h2 {
      margin-bottom: 20px;
      border-left: 6px solid #8d6e63;
      padding-left: 10px;
      color: #5d4037;
    }

    /* ================= CARDS ================= */
    .card {
      background: white;
      padding: 25px;
      border-radius: 12px;
      margin: 15px 0;
      box-shadow: 0 5px 15px rgba(0,0,0,0.15);
    }

    /* ================= BENEFÍCIOS ================= */
    .beneficios {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(200px,1fr));
      gap: 15px;
    }

    .beneficio {
      background: #8d6e63;
      color: white;
      padding: 20px;
      border-radius: 10px;
    }

    /* ================= GALERIA ================= */
    .galeria {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
      gap: 10px;
    }

    .galeria img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
    }

    /* ================= ACCORDION ================= */
    .accordion {
      width: 100%;
      padding: 15px;
      background: #6d4c41;
      color: white;
      border: none;
      text-align: left;
      margin-top: 10px;
      cursor: pointer;
      border-radius: 8px;
    }

    .panel {
      display: none;
      background: white;
      padding: 15px;
      border-radius: 0 0 8px 8px;
    }

    /* ================= BOTÃO ================= */
    .botao {
      padding: 12px 18px;
      background: #5d4037;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }

    /* ================= FOOTER ================= */
    footer {
      background: #3e2723;
      color: white;
      text-align: center;
      padding: 40px;
    }

    /* ================= ANIMAÇÃO ================= */
    @keyframes piscar {
      0% { transform: scale(1); }
      50% { transform: scale(1.03); }
      100% { transform: scale(1); }
    }

    /* ================= RESPONSIVO ================= */
    @media (max-width:768px) {
      header h1 { font-size: 2.5rem; }
      nav a { display: block; margin: 8px 0; }
    }
  </style>
</head>

<body>

<!-- ================= ENTRADA ================= -->
<div id="entrada">
  <h1>🌱 AGRO FORTE</h1>
  <p>Projeto educativo sobre sustentabilidade, tecnologia e o futuro do campo.</p>
  <button onclick="entrarSite()">Entrar</button>
</div>

<!-- ================= HEADER ================= -->
<header>
  <h1>AGRO FORTE</h1>
  <p>Um futuro melhor através da educação rural</p>
</header>

<!-- ================= MENU ================= -->
<nav>
  <a href="#sobre">Sobre</a>
  <a href="#beneficios">Benefícios</a>
  <a href="#animais">Animais</a>
  <a href="#galeria">Galeria</a>
  <a href="#interativo">Interativo</a>
</nav>

<!-- ================= SOBRE ================= -->
<section id="sobre">
  <h2>Sobre o Projeto</h2>
  <div class="card">
    <p>O projeto Agro Forte valoriza o campo, a tecnologia e a sustentabilidade no agronegócio moderno.</p>
  </div>
</section>

<!-- ================= BENEFÍCIOS ================= -->
<section id="beneficios">
  <h2>Benefícios</h2>

  <div class="beneficios">
    <div class="beneficio">Educação Rural</div>
    <div class="beneficio">Tecnologia</div>
    <div class="beneficio">Sustentabilidade</div>
    <div class="beneficio">Valorização do Campo</div>
  </div>
</section>

<!-- ================= ANIMAIS ================= -->
<section id="animais">
  <h2>Animais no Agro</h2>

  <div class="card">
    <p>Os animais são fundamentais para alimentação, economia e equilíbrio ambiental.</p>
  </div>
</section>

<!-- ================= GALERIA ================= -->
<section id="galeria">
  <h2>Galeria</h2>

  <div class="galeria">
    <img src="https://images.unsplash.com/photo-1500937386664-56d1dfef3854" />
    <img src="https://images.unsplash.com/photo-1500595046743-cd271d694d30" />
    <img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6" />
  </div>
</section>

<!-- ================= INTERATIVO ================= -->
<section id="interativo">
  <h2>Interativo</h2>

  <button class="accordion">O que é sustentabilidade?</button>
  <div class="panel"><p>Uso consciente dos recursos naturais.</p></div>

  <button class="accordion">Tecnologia no campo</button>
  <div class="panel"><p>Uso de drones, sensores e IA no agronegócio.</p></div>

  <div class="card">
    <button class="botao" onclick="mensagem()">Mensagem</button>
    <p id="msg"></p>
  </div>
</section>

<!-- ================= FOOTER ================= -->
<footer>
  <p>🌱 AGRO FORTE - Educação e Sustentabilidade</p>
</footer>

<!-- ================= SCRIPT ================= -->
<script>
  function entrarSite() {
    document.getElementById("entrada").style.display = "none";
  }

  function mensagem() {
    const textos = [
      "O futuro começa no campo 🌱",
      "Educação transforma o mundo 🚜",
      "Sustentabilidade é essencial 🌎"
    ];

    document.getElementById("msg").innerText =
      textos[Math.floor(Math.random() * textos.length)];
  }

  document.querySelectorAll(".accordion").forEach(btn => {
    btn.addEventListener("click", () => {
      const panel = btn.nextElementSibling;
      panel.style.display = panel.style.display === "block" ? "none" : "block";
    });
  });
</script>

</body>
</html>

# fisicaop
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Óptica Vibes - Duda Morici</title>
  <style>
    /* Reset básico */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: #e0e0e0;
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      position: fixed;
      top: 0; left: 0; right: 0;
      background: rgba(15, 32, 39, 0.95);
      box-shadow: 0 2px 8px rgba(0,0,0,0.7);
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      font-weight: 600;
      letter-spacing: 2px;
      font-size: 1.2rem;
      color: #f39c12;
    }
    header nav a {
      color: #f39c12;
      text-decoration: none;
      margin-left: 1.8rem;
      position: relative;
      transition: color 0.3s ease;
    }
    header nav a::after {
      content: '';
      position: absolute;
      width: 0%;
      height: 2px;
      background: #f39c12;
      bottom: -6px;
      left: 0;
      transition: 0.3s ease;
    }
    header nav a:hover, header nav a:focus {
      color: #ffc65c;
    }
    header nav a:hover::after {
      width: 100%;
    }

    main {
      padding: 120px 20px 40px;
      max-width: 900px;
      margin: 0 auto;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
      text-align: center;
      color: #ffc65c;
      text-shadow: 2px 2px 10px #f39c12;
    }
    h2 {
      margin-top: 3rem;
      margin-bottom: 1rem;
      color: #f39c12;
      border-bottom: 2px solid #f39c12;
      padding-bottom: 4px;
      font-weight: 700;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      filter: drop-shadow(0 0 3px #ffc65c);
    }

    p, ul {
      font-size: 1.1rem;
      margin-bottom: 1rem;
      color: #ddd;
    }

    ul {
      padding-left: 20px;
      list-style: none;
    }
    ul li {
      position: relative;
      padding-left: 1.2em;
      margin-bottom: 0.6em;
      cursor: default;
      transition: color 0.3s ease;
    }
    ul li::before {
      content: '⚡';
      position: absolute;
      left: 0;
      color: #f39c12;
      filter: drop-shadow(0 0 2px #f39c12);
      animation: pulse 2s infinite ease-in-out;
      top: 0.1em;
    }
    ul li:hover {
      color: #ffc65c;
    }

    @keyframes pulse {
      0%, 100% {opacity: 1;}
      50% {opacity: 0.5;}
    }

    /* Destaques em strong */
    strong {
      color: #ffc65c;
      font-weight: 700;
      text-shadow: 0 0 6px #f39c12;
    }

    /* Footer */
    footer {
      text-align: center;
      margin-top: 5rem;
      padding: 2rem 1rem;
      font-size: 0.9rem;
      color: #aaa;
      border-top: 1px solid #444;
      font-style: italic;
    }

    /* Scroll to top button */
    #toTopBtn {
      position: fixed;
      bottom: 30px;
      right: 30px;
      background: #f39c12;
      border: none;
      border-radius: 50%;
      width: 50px;
      height: 50px;
      cursor: pointer;
      box-shadow: 0 0 10px #f39c12;
      color: #121212;
      font-size: 2rem;
      display: none;
      align-items: center;
      justify-content: center;
      transition: background 0.3s ease;
      z-index: 1100;
    }
    #toTopBtn:hover {
      background: #ffc65c;
    }
    /* Responsividade */
    @media (max-width: 600px) {
      header {
        flex-direction: column;
        font-size: 1rem;
      }
      header nav a {
        margin: 0.5rem 0 0 0;
      }
    }
  </style>
</head>
<body>

<header>
  <div>Óptica Vibes</div>
  <nav>
    <a href="#luz">Luz</a>
    <a href="#comportamento">Comportamento</a>
    <a href="#lentes">Lentes & Espelhos</a>
    <a href="#imagem">Formação da Imagem</a>
    <a href="#fenomenos">Fenômenos</a>
    <a href="#aplicacoes">Aplicações</a>
  </nav>
</header>

<main>
  <h1>Óptica Simplificada na Real</h1>

  <section id="luz">
    <h2>Luz: o que é?</h2>
    <p>A luz é uma forma de energia que viaja em ondas — é o que permite a gente ver o mundo. Pode ser natural (tipo o sol que te acorda meio que com um tapa) ou artificial (aquele LED do seu celular que nunca desliga).</p>
  </section>

  <section id="comportamento">
    <h2>Como a luz se comporta?</h2>
    <p>A luz curte uns rolês específicos:</p>
    <ul>
      <li><strong>Reflexão:</strong> Quando a luz bate numa superfície e volta pra você, tipo seu reflexo no espelho daquele banheiro estiloso.</li>
      <li><strong>Refração:</strong> A luz muda o rumo quando passa de um meio pra outro, tipo quando o lápis na água parece estar torto — mó confusão pros olhos!</li>
      <li><strong>Absorção:</strong> A luz chega, bate e some — tipo quando sua bateria acaba e seu celular morre.</li>
      <li><strong>Transmissão:</strong> A luz atravessa materiais, como vidro, e segue seu caminho tranquilo.</li>
    </ul>
  </section>

  <section id="lentes">
    <h2>Lentes e Espelhos: o poder da distorção</h2>
    <p><strong>Espelhos</strong> refletem a luz e formam imagens que podem ser reais ou virtuais, dependendo do tipo (plano ou curvo). Já <strong>lentes</strong> são como “guardiões” que mudam o rumo da luz para ajudar você a enxergar melhor ou ampliar o que tá longe.</p>
    <ul>
      <li><strong>Lente convexa:</strong> junta os raios (tipo um encontro de crush), usada em lupas e óculos para quem enxerga longe mas tá meio confuso com o perto.</li>
      <li><strong>Lente côncava:</strong> espalha os raios (mais pra aquele amigo que gosta de espaço), usada em óculos para quem é míope e não vê longe.</li>
    </ul>
  </section>

  <section id="imagem">
    <h2>Formação da Imagem</h2>
    <p>Quando a luz passa por lentes ou reflete em espelhos, ela cria imagens que podem ser:</p>
    <ul>
      <li><strong>Reais:</strong> dá pra projetar numa tela, tipo cinema em casa.</li>
      <li><strong>Virtuais:</strong> só parecem reais, tipo aquela selfie com filtro que deixa tudo mais bonito.</li>
    </ul>
  </section>

  <section id="fenomenos">
    <h2>Fenômenos Ópticos que são um rolê à parte</h2>
    <ul>
      <li><strong>Dispersão:</strong> A luz branca se separa nas cores do arco-íris, tipo magia pura no céu depois da chuva.</li>
      <li><strong>Polarização:</strong> A luz vibra numa direção só, usada em óculos de sol pra você ficar estiloso e sem aquele brilho irritante.</li>
      <li><strong>Interferência e Difração:</strong> A luz se mistura e cria padrões coloridos, tipo as bolhas de sabão que você não consegue parar de olhar.</li>
    </ul>
  </section>

  <section id="aplicacoes">
    <h2>Pra que serve tudo isso?</h2>
    <p>- Câmeras, microscópios e telescópios, pra você registrar e explorar o universo.</p>
    <p>- Óculos pra deixar a visão tinindo, porque ninguém merece enxergar tudo embaçado.</p>
    <p>- Fibra óptica pra internet voando, nem dá tempo de piscar.</p>
    <p>- Laser, que corta, cura e até faz show de luz — tipo tecnologia com swag.</p>
  </section>

</main>

<button id="toTopBtn" title="Voltar ao topo">↑</button>

<script>
  // Mostrar botão voltar ao topo
  const toTopBtn = document.getElementById('toTopBtn');

  window.addEventListener('scroll', () => {
    if(window.scrollY > 300) {
      toTopBtn.style.display = 'flex';
    } else {
      toTopBtn.style.display = 'none';
    }
  });

  toTopBtn.addEventListener('click', () => {
    window.scrollTo({ top: 0, behavior: 'smooth' });
  });
</script>

</body>
</html>

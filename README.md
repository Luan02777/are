# Projeto do Alura Aeronautica
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Portfólio Aeronáutico</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(to bottom, #87ceeb, #fff);
      color: #333;
      overflow-x: hidden;
    }
    /* NUVENS PURAS EM CSS */
    .cloud {
      position: absolute;
      background: #fff;
      border-radius: 50%;
      box-shadow:
        40px 10px 0 0 #fff,
        80px 10px 0 0 #fff,
        20px 20px 0 0 #fff;
      width: 60px;
      height: 60px;
      animation: cloudMove 60s linear infinite;
      opacity: 0.7;
    }
    .cloud:nth-child(1) { top: 60px; left: -100px; animation-delay: 0s; }
    .cloud:nth-child(2) { top: 120px; left: -300px; animation-delay: 10s; }
    .cloud:nth-child(3) { top: 90px; left: -500px; animation-delay: 20s; }
    @keyframes cloudMove {
      0%   { transform: translateX(0); }
      100% { transform: translateX(150vw); }
    }
    /* AVIÃO ESTILIZADO */
    .plane {
      position: relative;
      width: 150px;
      height: 50px;
      margin: 60px auto 30px;
    }
    .plane::before {
      content: '';
      position: absolute;
      width: 100%;
      height: 20px;
      background: #222;
      border-radius: 10px;
      top: 15px;
    }
    .wing {
      position: absolute;
      width: 60px;
      height: 10px;
      background: #444;
      top: 0;
      left: 45px;
      transform: rotate(20deg);
      border-radius: 5px;
    }
    .tail {
      position: absolute;
      width: 20px;
      height: 20px;
      background: #444;
      top: 5px;
      left: 0;
      clip-path: polygon(0 0, 100% 0, 50% 100%);
    }
    /* CONTEÚDO */
    .container {
      max-width: 900px;
      margin: auto;
      background: rgba(255,255,255,0.9);
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.15);
      z-index: 1;
      position: relative;
    }
    header {
      text-align: center;
      margin-bottom: 30px;
    }
    header h1 {
      font-size: 2.5rem;
      color: #043102;
    }
    header p {
      font-size: 1.2rem;
      color: #13420c;
    }
    section {
      margin-bottom: 25px;
    }
    h2 {
      font-size: 1.6rem;
      color: #13420c;
      margin-bottom: 10px;
    }
    ul {
      padding-left: 20px;
    }
    ul li {
      margin-bottom: 8px;
    }
    footer {
      text-align: center;
      padding: 20px;
      color: #555;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <!-- Nuvens -->
  <div class="cloud"></div>
  <div class="cloud"></div>
  <div class="cloud"></div>

  <!-- Avião -->
  <div class="plane">
    <div class="wing"></div>
    <div class="tail"></div>
  </div>
  <!-- Conteúdo -->
  <div class="container">
    <header>
      <h1>Luan Pietro</h1>
      <p>Especialista em aeronaves e inovação tecnológica no setor aéreo</p>
    </header>
    <section>
      <h2>Sobre Mim</h2>
      <p>Sou engenheiro aeronáutico apaixonado por sistemas de propulsão e sustentabilidade na aviação. Desenvolvo projetos que unem eficiência e inovação.</p>
    </section>
    <section>
      <h2>Formação</h2>
      <ul>
        <li>Engenharia Aeronáutica - ITA</li>
      </ul>
    </section>
    <section>
      <h2>Experiência</h2>
      <ul>
        <li>Desenvolvimento de drones para transporte leve (2022 - atual)</li>
        <li>Consultoria em segurança de voo - AeroConsult (2018 - 2022)</li>
      </ul>
    </section>
    <section>
      <h2>Contato</h2>
      <p>Email: luanpietro@gmail.com</p>
      <p>Telefone: (11) 98956-4132</p>
    </section>
    <footer>
      &copy; 2025 Luan Pietro - Todos os direitos reservados.
    </footer>
  </div>
</body>
</html>****

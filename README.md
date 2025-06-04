<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>2 anos de namoro</title>
  <style>
    body {
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      font-family: 'Arial', sans-serif;
      color: #fff;
      text-align: center;
      padding: 50px;
      overflow: hidden;
    }

    h1 {
      font-size: 3em;
      margin-bottom: 20px;
    }

    #timer {
      font-size: 1.5em;
      margin-bottom: 50px;
    }

    .section {
      background: rgba(255, 255, 255, 0.2);
      margin: 20px auto;
      padding: 20px;
      border-radius: 15px;
      max-width: 600px;
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      transform: rotate(45deg);
      animation: float 10s infinite;
      opacity: 0.7;
    }

    .heart::before, .heart::after {
      content: '';
      position: absolute;
      width: 20px;
      height: 20px;
      background: red;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      left: -10px;
      top: 0;
    }

    @keyframes float {
      0% {
        transform: translateY(0) rotate(45deg);
        opacity: 0.7;
      }
      100% {
        transform: translateY(-100vh) rotate(45deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <h1>2 anos de namoro ❤️</h1>
  <div id="timer"></div>

  <div class="section">
    <h2>Como nos conhecemos</h2>
    <p>Nos conhecemos em um dia muito especial, cheio de coincidências que só o destino poderia explicar.</p>
  </div>

  <div class="section">
    <h2>Nossos momentos favoritos</h2>
    <p>Aquela viagem inesquecível, os jantares românticos e nossas risadas intermináveis.</p>
  </div>

  <div class="section">
    <h2>Nossos planos</h2>
    <p>Continuar construindo nossa história, viajando pelo mundo e sempre apoiando um ao outro.</p>
  </div>

  <script>
    const startDate = new Date("2023-07-02T00:00:00"); // Data do início do relacionamento

    function updateTimer() {
      const now = new Date();
      const diff = now - startDate;

      const seconds = Math.floor(diff / 1000) % 60;
      const minutes = Math.floor(diff / (1000 * 60)) % 60;
      const hours = Math.floor(diff / (1000 * 60 * 60)) % 24;
      const days = Math.floor(diff / (1000 * 60 * 60 * 24)) % 30;
      const months = Math.floor(diff / (1000 * 60 * 60 * 24 * 30)) % 12;
      const years = Math.floor(diff / (1000 * 60 * 60 * 24 * 365));

      document.getElementById('timer').innerHTML = `
        Estamos juntos há:<br>
        ${years} anos, ${months} meses, ${days} dias,<br>
        ${hours} horas, ${minutes} minutos e ${seconds} segundos
      `;
    }

    setInterval(updateTimer, 1000);
    updateTimer();

    // Gerar corações flutuantes
    for (let i = 0; i < 20; i++) {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (5 + Math.random() * 5) + 's';
      document.body.appendChild(heart);
    }
  </script>

</body>
</html>

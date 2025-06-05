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
      scroll-behavior: smooth;
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
      max-width: 700px;
      line-height: 1.8em;
      font-size: 1.1em;
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

  <h1>2 anos de namoro💕 - Julia Lyn</h1>
  <div id="timer"></div>

  <div class="section">
    <h2>Como nos conhecemos🤔</h2>
    <p>
      primeiramente eu gostaria de te falar UAU 2 ANOS EM,Nega que incrivel passar esses 2 anos ao seu lado, nosso encontro foi como o alinhamento perfeito das estrelas, inesperado e arrebatador. Desde o primeiro olhar, algo dentro de nós despertou e, sem perceber, começamos a construir algo maior do que nós mesmos: um amor puro, sincero e eterno. Cada conversa, cada risada e cada silêncio compartilhado nos uniu de uma forma inexplicável,aquele nosso primeiro beijo depois do treino me deixa louco só de pensar,foi incrivel demais,NUNCA me esquecerei
    </p>
  </div>

  <div class="section">
    <h2>Nossos momentos favoritos</h2>
    <p>
      Como esquecer das nossas longas caminhadas de mãos dadas, das tardes improvisados,das tardes preguiçosas em que simplesmente aproveitávamos a companhia um do outro? A cada data comemorada, a cada meta alcançada, nosso amor se fortaleceu, mostrando que somos mais felizes e completos quando estamos juntos,ainda nao fizemos uma viagem para deixar na memoria,mas logo logo a gente consegue
    </p>
  </div>

  <div class="section">
    <h2>Nossos planos🫠</h2>
    <p>
      O futuro nos espera com infinitas possibilidades e, ao seu lado, sei que qualquer caminho será mais leve, mais bonito e mais cheio de sentido. Queremos viajar o mundo, criar uma família, conquistar nossos sonhos e, acima de tudo, continuar aprendendo e crescendo um com o outro. Que nunca nos faltem motivos para sorrir, para abraçar e para celebrar a sorte de termos nos encontrado.
    </p>
  </div>

  <div class="section">
    <h2>Minha declaração😌</h2>
    <p>
      Quero que você saiba que te amo com toda a intensidade que cabe no meu coração. Você me inspira, me motiva e me completa. A sua presença torna meus dias mais felizes e me faz acreditar que o amor verdadeiro existe. Obrigado por ser meu porto seguro, minha melhor amiga, meu amor e minha paz. Que venham muitos e muitos anos ao seu lado, construindo a nossa história com carinho, respeito e muita cumplicidade. Te amo, para sempre!
    </p>
  </div>

  <div class="section">
    <h2>textinho🫦</h2>
    <p>
      Você me deixa completamente louca com esse seu jeito doce e safado ao mesmo tempo... 😏 Amo quando você me provoca com esse olhar malicioso, só para depois se fazer de inocente! 💋 Te desejo de um jeito tão intenso que mal consigo me concentrar quando penso em você... e penso o tempo todo! ❤️🔥 Mas, ao mesmo tempo, quero te encher de beijos, te abraçar forte e cuidar de você como ninguém. 💕 Você é minha tentação favorita e minha fofura mais preciosa. 😍 Nunca duvide: meu amor por você é tão grande quanto minha vontade de te agarrar e nunca mais soltar! 😘
    </p>
  </div>

  <div class="section">
    <h2>Minhas Promessas Para Você🥰</h2>
    <p>
      - Prometo sempre te surpreender com pequenos gestos de amor. 💝<br>
      - Prometo te ouvir com atenção, mesmo quando falar coisas bobas. 😂<br>
      - Prometo ser seu cúmplice em todas as aventuras. 🌍<br>
      - Prometo te abraçar forte sempre que precisar. 🤗<br>
      - Prometo fazer de cada dia ao seu lado o mais especial possível. ✨
    </p>
  </div>

  <div class="section">
    <h2>Um Poema Para Você😋</h2>
    <p>
      Nos teus olhos encontro abrigo,<br>
      No teu sorriso, meu destino.<br>
      Te desejo, te admiro, te provoco...<br>
      E te amo, cada dia um pouco mais.<br>
      Entre risadas, beijos e abraços,<br>
      Vamos seguindo, lado a lado,<br>
      E o que sinto por você, meu amor,<br>
      É eterno, sincero e apaixonado. ❤️
    </p>
  </div>

  <script>
    const startDate = new Date("2023-07-02T00:00:00");

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

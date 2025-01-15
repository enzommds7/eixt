<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Convite Especial</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(120deg, #f6d365, #fda085);
      color: #333;
      text-align: center;
      padding: 50px;
    }
    h1 {
      font-size: 2.5em;
      color: #fff;
    }
    p {
      font-size: 1.2em;
      color: #fff;
    }
    .button {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      font-size: 1.2em;
      color: #fff;
      background-color: #ff7b54;
      text-decoration: none;
      border-radius: 5px;
      transition: background-color 0.3s;
      cursor: pointer;
    }
    .button:hover {
      background-color: #ff5733;
    }
    #no-button {
      position: absolute;
      padding: 10px 20px;
      font-size: 1.2em;
      color: #fff;
      background-color: #f64c72;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: transform 0.3s;
    }
  </style>
</head>
<body>
  <h1>Oi, linda!</h1>
  <p>Queria fazer algo especial para te convidar para sair...</p>
  <p>O que acha de irmos fazer algo juntos qualquer dia desses?</p>
  
  <!-- Botão "Sim" -->
  <a href="https://youtu.be/WRHwuWC2W2g?si=yuUVBIVhUuWs_zWQ" target="_blank" class="button">Sim!</a>

  <!-- Botão "Não" -->
  <button id="no-button">Não</button>

  <script>
    const noButton = document.getElementById('no-button');

    noButton.addEventListener('mouseover', () => {
      const randomX = Math.floor(Math.random() * (window.innerWidth - 100));
      const randomY = Math.floor(Math.random() * (window.innerHeight - 50));
      noButton.style.position = 'absolute';
      noButton.style.left = randomX + 'px';
      noButton.style.top = randomY + 'px';
    });
  </script>
</body>
</html>
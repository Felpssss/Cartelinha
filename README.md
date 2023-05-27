# Cartelinha

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Meu Site</title>
  <style>
    /* Estilos globais */
    body {
      margin: 0;
      padding: 0;
      font-family: 'Quicksand', Arial, sans-serif;
    }
    
    /* Estilos para o cabeçalho */
    header {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      background-color: #ffffff;
      padding: 20px;
      border-bottom: 1px solid #EDEDED;
      color: #000000;
      font-weight: bold;
      text-align: center;
    }

    /* Estilos para o conteúdo */
    .container {
      margin-top: 80px; /* Considerando a altura do cabeçalho */
      background-color: #ffffff;
      padding: 20px;
    }
    
    /* Estilos para o botão amarelo */
    .button {
      position: fixed;
      bottom: 16px;
      left: 16px;
      right: 16px;
      background-color: #FEE500;
      color: #000000;
      padding: 15px;
      text-align: center;
      font-weight: bold;
      text-decoration: none;
      border-radius: 8px;
      overflow: hidden;
      transition: background-color 0.3s;
    }

    /* Estilos para o efeito de ripple ao clicar */
    .button::after {
      content: "";
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 100px;
      height: 100px;
      background-color: rgba(255, 255, 255, 0.3);
      border-radius: 50%;
      opacity: 0;
      pointer-events: none;
      animation: ripple 1s linear;
    }

    @keyframes ripple {
      0% {
        transform: translate(-50%, -50%) scale(0);
        opacity: 1;
      }
      100% {
        transform: translate(-50%, -50%) scale(2);
        opacity: 0;
      }
    }

    /* Estilos para o efeito de ripple ao clicar */
    .button:active::after {
      animation: none;
    }
  </style>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
  <header>
    Cartelas
  </header>

  <div class="container">
    <!-- Conteúdo da página aqui -->
  </div>
  
  <a href="#" class="button">Botão</a>
</body>
</html>

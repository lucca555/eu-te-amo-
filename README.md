<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para Você, Meu Amor</title>
    <style>
        body {
            background-color: #ffdde1;
            font-family: Arial, sans-serif;
            text-align: center;
            overflow: hidden;
            padding: 20px;
        }
        .mensagem {
            margin-top: 50px;
            font-size: 24px;
            color: #d63384;
            font-weight: bold;
        }
        .poema {
            font-size: 20px;
            color: #b22222;
            margin-top: 20px;
            font-style: italic;
        }
        .coracao {
            position: absolute;
            color: red;
            font-size: 20px;
            animation: cair 4s linear infinite;
        }
        @keyframes cair {
            0% { transform: translateY(-10vh); opacity: 1; }
            100% { transform: translateY(100vh); opacity: 0; }
        }
        .botao {
            background-color: #d63384;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 18px;
            cursor: pointer;
            border-radius: 10px;
            margin-top: 20px;
        }
        .imagem {
            display: none;
            margin-top: 20px;
            max-width: 90%;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <h1>Para Minha Princesa, Anna Clara 💖</h1>
    <p class="mensagem">Cada batida do meu coração é um "eu te amo" para você. ❤️</p>
    <p class="poema">
        Anna Clara, minha estrela, meu sol a brilhar,<br>
        Em teus olhos encontro o mar,<br>
        Teu sorriso ilumina meu dia,<br>
        És minha paz, minha alegria.<br><br>
        No teu abraço, o mundo silencia,<br>
        És meu sonho, minha poesia.<br>
        Para sempre ao teu lado quero estar,<br>
        Meu amor por ti jamais vai acabar. ❤️
    </p>
    <button class="botao" onclick="mostrarImagem()">Toque aqui para ver os olhos mais lindos do mundo 💖</button>
    <img id="imagemOlhos" class="imagem" src="https://i.imgur.com/TaiMPzI.jpeg" alt="Os olhos mais lindos do mundo">
    
    <script>
        function criarCoracao() {
            const coracao = document.createElement("div");
            coracao.classList.add("coracao");
            coracao.innerHTML = "❤️";
            coracao.style.left = Math.random() * 100 + "vw";
            coracao.style.animationDuration = (Math.random() * 2 + 3) + "s";
            document.body.appendChild(coracao);
            setTimeout(() => coracao.remove(), 4000);
        }
        setInterval(criarCoracao, 300);
        
        function mostrarImagem() {
            document.getElementById("imagemOlhos").style.display = "block";
        }
    </script>
</body>
</html>

<html>

<head>
    <title>ESTÁ SOZINHO?</title>

    <style>
        
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            text-align: center;
            height: 100vh;
            background-color: white;
            color: black;
            padding-top: 50px; 
        }

        h1, p {
            margin: 20px 0;
        }

        
        .paragrafo-grande {
            font-size: 24px;
        }

        .paragrafo-medio {
            font-size: 18px;
        }

        .paragrafo-pequeno {
            font-size: 12px;
        }

        
        #audioControl {
            margin-top: 20px; /* Dá espaço entre os textos e o botão */
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            font-size: 20px;
            padding: 20px;
            border: none;
            cursor: pointer;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(255, 0, 0, 0.5);
        }

        #audioControl:hover {
            background-color: rgba(255, 0, 0, 0.7);
        }

        
        img {
            position: absolute;
            right: 10px;
            top: 800px;
            width: 650px;
            height: 1200px;
        }
    </style>
</head>

<body>

    <audio id="audioPlayer" autoplay loop>
        <source src="boredman.mp3" type="audio/mp3">
        Seu navegador não suporta o formato de áudio.
    </audio>

    
    <p class="paragrafo-pequeno">VOCÊ PODE ME IGNORAR, MAS EU SEMPRE VOU ESTAR PRESENTE. OLHE AO SEU REDOR, NÃO ESTOU LONGE...</p>
    <h1>SIM, VOCÊ NÃO LEU ERRADO O NOME DA ABA DO SITE...</h1>
    <p class="paragrafo-grande">ESTOU PERGUNTANDO POR QUE FICAREI TRISTE SE VOCÊ DISSER QUE SIM, POIS ESTARÁ DIZENDO QUE NÃO ACREDITA EM MIM, NÃO ESTÁ ME SENTINDO NA JANELA?...</p>
    <p class="paragrafo-medio">A CADA DIA QUE PASSA, EU OBSERVO VOCÊ. ACHO QUE VOCÊ NÃO PERCEBE, MAS EU ESTOU AQUI...</p>

   
    <button id="audioControl" onclick="toggleAudio()">Clique aqui para me ouvir</button>

   
    <img src="bixo.png" alt="EU PODERIA MOSTRAR COMO EU SOU">

    <script>
        
        function toggleAudio() {
            var audio = document.getElementById("audioPlayer");
            if (audio.paused) {
                audio.play();
                document.getElementById("audioControl").innerText = "Agora é tarde";
            } else {
                audio.pause();
                document.getElementById("audioControl").innerText = "Clique aqui para me ouvir";
            }
        }
    </script>

</body>

</html>

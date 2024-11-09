<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surprise Fun</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 100px;
        }

        .message {
            font-size: 24px;
            color: #ff6347;
            padding: 20px;
            border: 2px solid #ff6347;
            border-radius: 10px;
            background-color: #fff5e6;
        }

        .popup {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            padding: 30px;
            border-radius: 10px;
            background-color: #ffcccb;
            border: 3px solid #ff6347;
            display: none;
            z-index: 1000;
        }
    </style>
</head>
<body>
    <h1>Surprise ! 😜</h1>
    <p>Prépare-toi à être surpris !</p>

    <!-- Message principal -->
    <div class="message">
        Clique ici pour voir la surprise !
    </div>

    <!-- Popup de la surprise -->
    <div class="popup" id="popup">
        <h2>🎉 Surprise ! 🎉</h2>
        <p>Tu es tombé dans le piège ! 😜</p>
    </div>

    <script>
        // Fonction pour afficher le popup
        document.querySelector('.message').addEventListener('click', function() {
            var popup = document.getElementById('popup');
            popup.style.display = 'block';
            setTimeout(function() {
                popup.style.display = 'none'; // Cache le popup après 3 secondes
            }, 3000);
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Message Rigolo</title>
</head>
<body>

    <h1>Clique ici pour une surprise !</h1>
    <button onclick="showFunnyAlert()">Cliquez-moi !</button>

    <script>
        function showFunnyAlert() {
            alert("Fait pas confiance au site comme celui-ci mon grand, c'est dangereux ! ⚠️");
        }
    </script>

</body>
</html>
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Texte Rigolo</title>
    <style>
        body {
            text-align: center;
            margin-top: 100px;
            font-family: Arial, sans-serif;
        }

        #funnyText {
            font-size: 30px;
            transition: all 0.5s ease;
        }
    </style>
</head>
<body>

    <h1 id="funnyText">Tu me vois ? 😜</h1>

    <script>
        // Change la couleur du texte et sa position à chaque clic
        document.getElementById('funnyText').addEventListener('click', function() {
            var colors = ['#FF6347', '#00BFFF', '#32CD32', '#FFD700', '#FF69B4'];
            var randomColor = colors[Math.floor(Math.random() * colors.length)];
            var randomX = Math.random() * window.innerWidth;
            var randomY = Math.random() * window.innerHeight;

            this.style.color = randomColor;
            this.style.position = 'absolute';
            this.style.left = randomX + 'px';
            this.style.top = randomY + 'px';
        });
    </script>

</body>
</html>

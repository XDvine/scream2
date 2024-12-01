<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Скример</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            overflow: hidden;
            width: 100%;
            height: 100%;
            background: black;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
        }

        #screamer {
            display: none;
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: black;
            justify-content: center;
            align-items: center;
        }

        #screamer img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    </style>
</head>
<body>
    <div id="screamer">
        <img src="https://via.placeholder.com/1920x1080/FF0000/FFFFFF?text=Scream!" alt="Scary Image">
    </div>

    <audio id="screamSound" src="scream.mp3"></audio>

    <script>
        document.body.addEventListener('click', function () {
            // Показать скример
            const screamer = document.getElementById('https://png.klev.club/uploads/posts/2024-03/png-klev-club-p-skrimer-png-24.png');
            const screamSound = document.getElementById('screamSound');

            screamer.style.display = 'flex';
            screamSound.play();

            // Удалить через 3 секунды
            setTimeout(() => {
                screamer.style.display = 'none';
            }, 3000);
        });
    </script>
</body>
</html>

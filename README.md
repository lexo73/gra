<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gra klikana</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }

        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 20px;
            cursor: pointer;
        }

        #score {
            font-size: 24px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Gra klikana</h1>
    <p>Klikaj przycisk, aby zdobywać punkty!</p>
    <div id="score">Punkty: 0</div>
    <button id="clickButton">Kliknij mnie!</button>

    <script>
        let score = 0;

        const scoreElement = document.getElementById('score');
        const clickButton = document.getElementById('clickButton');

        clickButton.addEventListener('click', () => {
            score++;
            scoreElement.textContent = `Punkty: ${score}`;
        });
    </script>
</body>
</html>

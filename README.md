# Enigma<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indovinello: Chi sono?</title>
    <style>
        body {
            background-color: #333;
            color: white;
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 100px;
        }
        input[type="text"] {
            padding: 10px;
            margin: 10px;
        }
        #message {
            margin-top: 20px;
            font-size: 18px;
            color: green;
        }
    </style>
</head>
<body>
    <h1>Indovinello: Chi sono?</h1>
    <p>Ho 24 anni, adoro leggere e la mia pizza preferita è la margherita. Chi sono?</p>
    <input type="text" id="answer" placeholder="Scrivi la tua risposta">
    <button onclick="checkAnswer()">Controlla</button>
    <p id="message"></p>

    <script>
        function checkAnswer() {
            var userAnswer = document.getElementById("answer").value.toLowerCase();
            var correctAnswer = "ale"; // risposta corretta

            if (userAnswer === correctAnswer) {
                document.getElementById("message").innerHTML = "Esatto! Sono Ale, una persona che ama i libri e la pizza!";
            } else {
                document.getElementById("message").innerHTML = "Sbagliato, prova ancora!";
            }
        }
    </script>
</body>
</html>

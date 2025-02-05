# san-valentin
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Mi Conicita, quieres ser mi San Valentín?</title>
    <style>
        @keyframes floating-hearts {
            0% { transform: translateY(0) scale(1); opacity: 1; }
            100% { transform: translateY(-100vh) scale(1.5); opacity: 0; }
        }

        body {
            background-color: #ffe6e6;
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }

        .container {
            position: relative;
            padding: 20px;
            z-index: 10;
        }

        h1 {
            color: #ff3366;
            font-size: 2.5em;
            margin-top: 50px;
            animation: fadeIn 2s ease-in-out;
        }

        p {
            color: #333;
            font-size: 1.2em;
            margin: 20px 0;
        }

        .button {
            background-color: #ff3366;
            color: #fff;
            padding: 15px 30px;
            text-decoration: none;
            font-size: 1.2em;
            border-radius: 25px;
            margin: 10px;
            display: inline-block;
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease-in-out;
        }

        .button:hover {
            background-color: #e62e5c;
            transform: scale(1.1);
        }

        .heart {
            position: absolute;
            bottom: -50px;
            left: 50%;
            font-size: 30px;
            color: #ff3366;
            animation: floating-hearts 5s linear infinite;
        }
        
        /* Generar corazones aleatorios */
        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.8); }
            to { opacity: 1; transform: scale(1); }
        }
        
        .heart:nth-child(1) { left: 10%; animation-duration: 4s; }
        .heart:nth-child(2) { left: 25%; animation-duration: 5s; }
        .heart:nth-child(3) { left: 40%; animation-duration: 6s; }
        .heart:nth-child(4) { left: 55%; animation-duration: 7s; }
        .heart:nth-child(5) { left: 70%; animation-duration: 5s; }
        .heart:nth-child(6) { left: 85%; animation-duration: 6s; }
    </style>
</head>
<body>
    <div class="container">
        <h1>¿Mi Conicita, quieres ser mi San Valentín? 💖</h1>
        <p>Me harías muy feliz si aceptas ser mi compañía en este día tan especial.</p>
        <a href="#" class="button">Sí 💕</a>
        <a href="#" class="button">No 💔</a>
    </div>

    <!-- Corazones flotantes -->
    <script>
        for (let i = 0; i < 10; i++) {
            let heart = document.createElement("div");
            heart.innerHTML = "❤️";
            heart.classList.add("heart");
            document.body.appendChild(heart);
        }
    </script>
</body>
</html>

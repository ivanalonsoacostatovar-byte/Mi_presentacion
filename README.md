<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Presentación Interactiva</title>
    <link href="https://fonts.googleapis.com/css2?family=Righteous&family=Poppins:wght@300;600&display=swap" rel="stylesheet">
    <style>
        /* Fondo animado Aurora */
        body { 
            margin: 0; 
            height: 100vh; 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            font-family: 'Poppins', sans-serif; 
            background: linear-gradient(-45deg, #ff00c1, #9600ff, #4900ff, #00b8ff, #00fff9); 
            background-size: 400% 400%; 
            animation: aurora 15s ease infinite; 
            overflow: hidden; 
        }

        @keyframes aurora { 
            0% { background-position: 0% 50%; } 
            50% { background-position: 100% 50%; } 
            100% { background-position: 0% 50%; } 
        }

        /* Tarjeta de cristal */
        .card { 
            text-align: center; 
            background: rgba(0, 0, 0, 0.4); 
            padding: 50px; 
            border-radius: 40px; 
            backdrop-filter: blur(20px); 
            border: 1px solid rgba(255, 255, 255, 0.2); 
            width: 90%; 
            max-width: 500px; 
            box-shadow: 0 25px 50px rgba(0,0,0,0.3);
        }

        h1 { 
            font-family: 'Righteous', cursive; 
            color: #fff; 
            text-shadow: 0 0 20px #ff00c1; 
            margin-bottom: 20px; 
            transition: 0.5s;
        }

        /* Botón Neón */
        .btn-neon { 
            padding: 20px 40px; 
            color: #fff; 
            text-decoration: none; 
            border: 3px solid #00fff9; 
            border-radius: 50px; 
            display: inline-block; 
            font-weight: bold; 
            transition: 0.3s; 
            position: relative;
            overflow: hidden;
        }

        .btn-neon:hover { 
            background: #00fff9; 
            color: #000; 
            box-shadow: 0 0 40px #00fff9; 
            transform: scale(1.1); 
        }
    </style>
</head>
<body>

    <div class="card">
        <h1 id="main-title">Ir a la Presentación</h1>
        <p style="color: white; margin-bottom: 30px;">Haz clic para ver el contenido en Google Drive.</p>
        
        <a href="https://docs.google.com/presentation/d/1pDgXC7q2luZtWnFwTKjcegCLPoB9zJDB13v-wp3dImQ/edit?usp=sharing" 
           class="btn-neon" 
           id="action-btn"
           target="_blank">
            ¡Ver Ahora!
        </a>
    </div>

    <script src="script.js"></script>
</body>
</html>


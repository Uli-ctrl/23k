<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Te casarías conmigo?</title>
    <style>
        body {
            text-align: center;
            background-color: #f8e1e7;
            font-family: Arial, sans-serif;
        }
        .container {
            margin-top: 50px;
        }
        h1 {
            color: #d63384;
        }
        .gallery {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }
        img {
            width: 200px;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            background-color: #ff4081;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 20px;
            cursor: pointer;
            border-radius: 5px;
        }
        button:hover {
            background-color: #d81b60;
        }
        #no {
            position: absolute;
        }
    </style>
</head>
<body>
    <audio autoplay loop>
        <source src="musica.mp3" type="audio/mpeg">
    </audio>
    <div class="container">
        <h1>¿Te casarías conmigo?</h1>
        <p>Desde que te conocí, supe que eras la persona con la que quiero compartir mi vida,perdon hacerte renegar por hacerte estar mal pero esta bien quiero hacer bie y compartir mi vida con vos ❤️</p>
        <div class="gallery">
            <img src="foto1.jpg" alt="Nosotros">
            <img src="foto2.jpg" alt="Juntos">
            <img src="foto3.jpg" alt="Amor">
        </div>
        <div class="buttons">
            <button onclick="alert('¡Sabía que dirías que sí! ❤️')">Sí</button>
            <button id="no" onmouseover="moverBoton()">No</button>
        </div>
    </div>
    <script>
        function moverBoton() {
            let botonNo = document.getElementById("no");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            botonNo.style.left = `${x}px`;
            botonNo.style.top = `${y}px`;
        }
    </script>
</body>
</html>

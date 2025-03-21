<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para mi niña, mi amor, mi reina</title>
    <style>
        body {
            font-family: 'Georgia', serif;
            background-color: #fff5e1;
            color: #4a4a4a;
            margin: 0;
            padding: 0;
            overflow: hidden;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            text-align: center;
            position: relative;
            z-index: 1;
        }
        h1 {
            font-size: 3rem;
            color: #e67e22;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.2rem;
            line-height: 1.6;
            margin-bottom: 20px;
        }
        .hearts, .flowers {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }
        .hearts span, .flowers span {
            position: absolute;
            display: block;
            animation: animate 10s linear infinite;
        }
        .hearts span {
            color: #ff6b6b;
            font-size: 2rem;
        }
        .flowers span {
            color: #f1c40f;
            font-size: 3rem;
        }
        @keyframes animate {
            0% {
                transform: translateY(-10%);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(110%);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="hearts">
        <span>❤️</span>
        <span>❤️</span>
        <span>❤️</span>
        <span>❤️</span>
        <span>❤️</span>
    </div>
    <div class="flowers">
        <span>🌼</span>
        <span>🌼</span>
        <span>🌼</span>
        <span>🌼</span>
        <span>🌼</span>
    </div>
    <div class="container">
        <h1>Para mi niña, mi amor, mi reina</h1>
        <p>
            Mi niña, mi amor, mi reina... No hay palabras suficientes para expresar lo mucho que te amo. Desde el momento en que entraste en mi vida, todo cobró un nuevo sentido. Eres la luz que ilumina mis días, la razón por la que sonrío sin motivo y la persona que hace que todo valga la pena.
        </p>
        <p>
            Me encanta estar contigo, compartir risas, sueños y hasta esos momentos de silencio en los que simplemente estamos juntos. Eres mi compañera, mi confidente, mi mejor amiga. Agradezco a la vida por haberte puesto en mi camino, porque contigo he aprendido lo que es el amor verdadero.
        </p>
        <p>
            Confío en ti, en nosotros, en este amor que construimos día a día. Deseo una vida a tu lado, amándote, cuidándote y haciéndote muy feliz. Eres mi todo, mi razón de ser, y prometo estar contigo en las buenas y en las malas, siempre.
        </p>
        <p>
            Te amo más de lo que las palabras pueden expresar. Eres mi niña, mi amor, mi reina, y siempre lo serás. 💛🌼
        </p>
    </div>
    <script>
        // Función para crear corazones y flores dinámicamente
        function createHeartsAndFlowers() {
            const heartsContainer = document.querySelector('.hearts');
            const flowersContainer = document.querySelector('.flowers');

            for (let i = 0; i < 20; i++) {
                const heart = document.createElement('span');
                heart.innerHTML = '❤️';
                heart.style.left = Math.random() * 100 + 'vw';
                heart.style.animationDuration = Math.random() * 5 + 5 + 's';
                heartsContainer.appendChild(heart);

                const flower = document.createElement('span');
                flower.innerHTML = '🌼';
                flower.style.left = Math.random() * 100 + 'vw';
                flower.style.animationDuration = Math.random() * 5 + 5 + 's';
                flowersContainer.appendChild(flower);
            }
        }

        createHeartsAndFlowers();
    </script>
</body>
</html>

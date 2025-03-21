!DOCTYPE html>
 <html lang="es">
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Para mi Amor</title>
   <style>
     body {
       font-family: 'Georgia', serif;
       background: linear-gradient(135deg, #f9f7f7, #e3f2fd);
       color: #333;
       text-align: center;
       margin: 0;
       padding: 20px;
       min-height: 100vh;
       display: flex;
       flex-direction: column;
       justify-content: center;
       align-items: center;
       position: relative;
       overflow: auto; /* Permitir scroll */
     }
 
     /* Fondo con flores sutiles */
     body::before {
       content: '';
       position: absolute;
       top: 0;
       left: 0;
       width: 100%;
       height: 100%;
       background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 200'%3E%3Cpath fill='%23ffeb3b' opacity='0.1' d='M50 100c0-27.6 22.4-50 50-50s50 22.4 50 50-22.4 50-50 50-50-22.4-50-50zm50-80c-44.2 0-80 35.8-80 80s35.8 80 80 80 80-35.8 80-80-35.8-80-80-80z'/%3E%3C/svg%3E");
       background-size: 100px;
       opacity: 0.3;
       z-index: -1;
     }
 
     h1 {
       font-size: 2.5rem;
       margin-bottom: 15px;
       color: #e91e63;
     }
 
     p {
       font-size: 1.2rem;
       max-width: 90%;
       line-height: 1.6;
       margin-bottom: 20px;
     }
 
     .flower {
       font-size: 4rem;
       margin-top: 20px;
       transition: color 1s ease;
     }
 
     /* Estilos responsivos */
     @media (max-width: 600px) {
       h1 {
         font-size: 2rem;
       }
       p {
         font-size: 1rem;
       }
       .flower {
         font-size: 3rem;
       }
     }
   </style>
 </head>
 <body>
   <h1>Para mi Amor 💖</h1>
   <p>
     Mi niña, cada día a tu lado es como una página nueva en el libro más hermoso que he leído. 
     Eres la protagonista de mi historia, la razón por la que mi corazón late con tanta fuerza. 
     Desde que llegaste a mi vida, todo cobró sentido, como si el universo hubiera estado preparando este momento solo para nosotros. <br>
 
     Mi vida, eres la luz que ilumina mis días más oscuros. Con tu sonrisa, el mundo parece detenerse, 
     y solo existes tú y yo. Eres mi refugio, mi paz, mi razón para sonreír incluso en los días más difíciles. 
     Contigo, todo es más bonito, más cálido, más lleno de amor.<br>
 
     Mi amor, no hay palabras suficientes para describir lo que siento por ti. Eres esa flor que crece en el jardín de mi corazón, 
     cuidada con todo el cariño que soy capaz de dar. Cada día que pasa, mi amor por ti crece más y más, como si no hubiera límites
     para todo lo que puedo sentir por ti. <br>
 
     Mi amor prometo amarte hoy, mañana y siempre. Eres mi sueño hecho realidad, mi eterna complicidad, mi razón para creer en el amor. 
     Te amo más de lo que las palabras pueden expresar, y estoy agradecido por cada instante a tu lado.<br>
 
     Con todo mi corazón,<br>
     Tu amor que te adora. 💖
   </p>
   <div class="flower" id="flower">🌺</div>
 
   <script>
     // Fecha objetivo: 21 de marzo de 2025
     const targetDate = new Date('2025-03-21T00:00:00');
     const startDate = new Date(); // Fecha de inicio (hoy)
 
     // Función para calcular el color de la flor
     function getFlowerColor() {
       const now = new Date();
       if (now >= targetDate) {
         return 'yellow'; // Flores amarillas a partir del 21 de marzo de 2025
       } else {
         const totalTime = targetDate - startDate; // Tiempo total entre hoy y la fecha objetivo
         const elapsedTime = now - startDate; // Tiempo transcurrido desde hoy
         const percent = (elapsedTime / totalTime) * 100; // Porcentaje de progreso
 
         // Ajustar el color gradualmente (de rojo a amarillo)
         const red = Math.floor(255 - (percent * 2.55));
         const green = Math.floor(percent * 2.55);
         return `rgb(${red}, ${green}, 0)`;
       }
     }
 
     // Aplicar el color a la flor
     const flowerElement = document.getElementById('flower');
     flowerElement.style.color = getFlowerColor();
 
     // Actualizar el color cada día
     setInterval(() => {
       flowerElement.style.color = getFlowerColor();
     }, 1000 * 60 * 60 * 24); // Actualizar cada 24 horas
   </script>
 </body>
 </html>

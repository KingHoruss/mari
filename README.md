<!DOCTYPE html>
<html>
<head>
    <title>💖 Regalo especial 14 Febrero 💖</title>
    <meta charset="UTF-8">
    <style>
        body { 
            background: linear-gradient(45deg, #ff69b4, #ff1493, #c71585); 
            font-family: 'Comic Sans MS', cursive; 
            text-align: center; 
            color: white; 
            margin: 0; 
            padding: 20px;
            min-height: 100vh;
        }
        h1 { font-size: 2.5em; text-shadow: 2px 2px 4px rgba(0,0,0,0.5); }
        .corazon { font-size: 1.2em; margin: 40px auto; max-width: 400px; }
        .mensaje { font-size: 1.5em; margin-top: 40px; line-height: 1.6; }
        input { font-size: 1.2em; padding: 15px; border: none; border-radius: 25px; width: 250px; }
        button { font-size: 1.2em; padding: 15px 30px; background: white; color: #ff1493; border: none; border-radius: 25px; cursor: pointer; margin-top: 20px; }
        button:hover { background: #ffd1dc; transform: scale(1.05); }
    </style>
</head>
<body>
    <h1>💝 ¡Sorpresa del 14 de febrero! 💝</h1>
    
    <div class="corazon">
<pre>
     *****       *****
   *********   *********
  *********** ***********
  ************************
  ************************
   **********************
    ********************
      ****************
        ************
          ********
            ****
             **
</pre>
    </div>
    
    <input id="nombre" placeholder="Escribe tu nombre, amor 💕" type="text">
    <br>
    <button onclick="mostrarAmor()">Ver mi mensaje especial ❤️</button>
    
    <div id="mensaje" class="mensaje" style="display:none;"></div>

    <script>
        function mostrarAmor() {
            let nombre = document.getElementById('nombre').value || 'mi amor más bonito';
            let msg = document.getElementById('mensaje');
            msg.style.display = 'block';
            msg.innerHTML = 
                `¡Feliz 14 de febrero, <strong style="color:gold;">${nombre}</strong>! 🌹<br><br>` +
                `Este corazoncito lo he programado yo pensando en ti.<br>` +
                `Cada símbolo es un poquito de lo mucho que te quiero.<br>` +
                `Eres mi mundo entero 💖`;
            
            // Efecto corazones volando
            for(let i=0; i<20; i++) {
                setTimeout(() => {
                    let corazon = document.createElement('div');
                    corazon.innerHTML = '💖';
                    corazon.style.position = 'fixed';
                    corazon.style.left = Math.random()*100 + 'vw';
                    corazon.style.animation = 'float 3s ease-out forwards';
                    document.body.appendChild(corazon);
                    setTimeout(() => corazon.remove(), 3000);
                }, i*100);
            }
        }
    </script>

    <style>
        @keyframes float {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-100px) rotate(360deg); opacity: 0; }
        }
    </style>
</body>
</html>
# mari

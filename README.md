# diarioavanzado
diario V2
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Contador de Clicks</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 50px;
    }
    #contador {
      font-size: 48px;
      margin: 20px 0;
    }
    button {
      font-size: 24px;
      padding: 10px 20px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <h1>Contador de Clicks</h1>
  <div id="contador">0</div>
  <button id="botonContar">Haz Click</button>
  <button id="botonReset">Reiniciar</button>

  <script>
    // Obtener referencias a los elementos del DOM
    const contador = document.getElementById('contador');
    const botonContar = document.getElementById('botonContar');
    const botonReset = document.getElementById('botonReset');

    // Variable para contar los clics
    let cuenta = 0;

    // Evento para incrementar el contador
    botonContar.addEventListener('click', () => {
      cuenta++;
      contador.textContent = cuenta;
    });

    // Evento para reiniciar el contador
    botonReset.addEventListener('click', () => {
      cuenta = 0;
      contador.textContent = cuenta;
    });
  </script>

</body>
</html>
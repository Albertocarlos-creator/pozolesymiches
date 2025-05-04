
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Miches y Pozoles</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff8f0;
      color: #333;
    }
    header, footer {
      background-color: #b22222;
      color: white;
      text-align: center;
      padding: 1.5rem;
    }
    nav {
      background-color: #8b0000;
      text-align: center;
      padding: 0.5rem;
    }
    nav a {
      color: white;
      margin: 0 1rem;
      text-decoration: none;
      font-weight: bold;
      cursor: pointer;
    }
    .hero {
      background-color: #e57373;
      color: white;
      padding: 4rem 2rem;
      text-align: center;
    }
    .section {
      padding: 2rem;
      text-align: center;
    }
    .menu {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
    .menu-item {
      background-color: #fff;
      border: 1px solid #ddd;
      border-radius: 10px;
      margin: 1rem;
      padding: 1rem;
      width: 250px;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>

  <header>
    <h1>Miches y Pozoles</h1>
    <p>El mejor sabor mexicano en un solo lugar</p>
  </header>

  <nav>
    <a onclick="mostrarSeccion('inicio')">Inicio</a>
    <a onclick="mostrarSeccion('menu')">Menú</a>
    <a onclick="mostrarSeccion('contacto')">Contacto</a>
  </nav>

  <!-- SECCIÓN INICIO -->
  <div id="inicio">
    <section class="hero">
      <h1>¡Disfruta un buen pozole con una michelada!</h1>
    </section>

    <section class="section">
      <h2>Sobre Nosotros</h2>
      <p>En "Miches y Pozoles" celebramos la tradición mexicana con los sabores más auténticos de pozole y micheladas. Todo hecho con amor y sazón.</p>
    </section>
  </div>

  <!-- SECCIÓN MENÚ -->
  <div id="menu" class="hidden">
    <section class="section">
      <h2>Menú Principal</h2>
      <div class="menu">
        <div class="menu-item">
          <h3>Pozole Rojo</h3>
          <p>Hecho con chile guajillo y carne de cerdo.</p>
          <strong>$120 MXN</strong>
        </div>
        <div class="menu-item">
          <h3>Pozole Verde</h3>
          <p>Con carne de pollo y salsa verde casera.</p>
          <strong>$120 MXN</strong>
        </div>
        <div class="menu-item">
          <h3>Pozole Blanco</h3>
          <p>Estilo tradicional con rábano, lechuga y orégano.</p>
          <strong>$115 MXN</strong>
        </div>
        <div class="menu-item">
          <h3>Michelada Clásica</h3>
          <p>Cerveza, limón, salsas y escarchado con sal y chile.</p>
          <strong>$75 MXN</strong>
        </div>
        <div class="menu-item">
          <h3>Quesadillas</h3>
          <p>De queso o combinadas, acompañadas con guacamole.</p>
          <strong>$60 MXN</strong>
        </div>
      </div>
    </section>
  </div>

  <!-- SECCIÓN CONTACTO -->
  <div id="contacto" class="hidden">
    <section class="section">
      <h2>Contacto</h2>
      <p>📍 Av. Sabor Mexicano #123, CDMX</p>
      <p>📞 55-1234-5678</p>
      <p>✉️ contacto@michesypozoles.mx</p>
    </section>
  </div>

  <footer>
    <p>&copy; 2025 Miches y Pozoles. Todos los derechos reservados.</p>
  </footer>

  <script>
    function mostrarSeccion(seccionId) {
      const secciones = ['inicio', 'menu', 'contacto'];
      secciones.forEach(id => {
        document.getElementById(id).classList.add('hidden');
      });
      document.getElementById(seccionId).classList.remove('hidden');
    }
  </script>

</body>
</html>

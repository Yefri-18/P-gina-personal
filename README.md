<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de Presentación</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #1a1a1a, #333);
            color: #f5f5f5;
            line-height: 1.6;
            overflow-x: hidden;
        }

        header {
            background: url('https://www.example.com/amigable-background.jpg') no-repeat center center/cover;
            color: white;
            padding: 80px 0;
            text-align: center;
            font-size: 3em;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav a {
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            font-weight: bold;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        nav a:hover {
            background-color: #e91e63;
            transform: scale(1.1);
        }

        section {
            padding: 60px 20px;
            max-width: 1200px;
            margin: auto;
            animation: fadeInUp 1s ease-in-out;
        }

        .section-title {
            color: #e91e63;
            font-size: 2.5em;
            margin-bottom: 30px;
            text-align: center;
            text-transform: uppercase;
            letter-spacing: 1px;
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 60px;
            height: 4px;
            background-color: #ff4081;
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }

        .proyectos {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .proyecto {
            background-color: #444;
            border-radius: 10px;
            padding: 30px;
            transition: transform 0.3s ease, background-color 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            text-decoration: none;
            color: #f5f5f5;
        }

        .proyecto:hover {
            transform: translateY(-15px);
            background-color: #555;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
        }

        .proyecto h3 {
            color: #ff9800;
            margin-bottom: 15px;
            font-size: 1.5em;
        }

        .contacto {
            background-color: #03a9f4;
            border-radius: 10px;
            padding: 40px;
            color: #fff;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .contacto:hover {
            transform: translateY(-15px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
        }

        .contacto a {
            color: #fff;
            text-decoration: underline;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        .contacto a:hover {
            color: #ff4081;
        }

        .social-icons {
            margin-top: 20px;
        }

        .social-icons a {
            margin: 0 10px;
            display: inline-block;
            color: white;
            font-size: 2em;
            transition: transform 0.3s ease, color 0.3s ease;
        }

        .social-icons a:hover {
            color: #ff4081;
            transform: scale(1.2);
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            box-shadow: 0 -4px 10px rgba(0, 0, 0, 0.2);
            position: relative;
        }

        @keyframes fadeInUp {
            0% {
                opacity: 0;
                transform: translateY(20px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>

<header>
    <h1>Bienvenido a Mi Página Personal</h1>
</header>

<nav>
    <a href="#proyectos">Proyectos</a>
    <a href="#contacto">Contacto</a>
</nav>

<section id="proyectos">
    <h2 class="section-title">Proyectos</h2>
    <div class="proyectos">
        <a href="https://www.example.com/proyecto1" class="proyecto">
            <h3>Proyecto 1</h3>
            <p>Descripción breve del Proyecto 1.</p>
        </a>
        <a href="https://www.example.com/proyecto2" class="proyecto">
            <h3>Proyecto 2</h3>
            <p>Descripción breve del Proyecto 2.</p>
        </a>
        <a href="https://www.example.com/proyecto3" class="proyecto">
            <h3>Proyecto 3</h3>
            <p>Descripción breve del Proyecto 3.</p>
        </a>
    </div>
</section>

<section id="contacto">
    <h2 class="section-title">Contacto</h2>
    <div class="contacto">
        <p>Puedes ponerte en contacto conmigo enviándome un <a href="mailto:tuemail@ejemplo.com">correo electrónico</a> o seguirme en mis redes sociales.</p>
        <div class="social-icons">
            <a href="https://twitter.com/tuperfil" target="_blank"><i class="fab fa-twitter"></i></a>
            <a href="https://www.linkedin.com/in/tuperfil" target="_blank"><i class="fab fa-linkedin"></i></a>
            <a href="https://github.com/tuperfil" target="_blank"><i class="fab fa-github"></i></a>
            <a href="https://www.instagram.com/tuperfil" target="_blank"><i class="fab fa-instagram"></i></a>
        </div>
    </div>
</section>

<footer>
    <p>&copy; 2024 Tu Nombre. Todos los derechos reservados.</p>
</footer>

</body>
</html>

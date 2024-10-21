<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biografía</title>
    <style>
        /* Reseteo de márgenes */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        /* Estilos generales */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: rgb(226, 222, 222);
            background-color: rgb(0, 38, 77);
        }
        /* Contenedor */
        .container {
            width: 80%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
        }
        .container2 {
            width: 80%;
            margin: 0 auto;
            display: block;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        /* Encabezado */
        #main-header {
            position: fixed;
            width: 100%;
            top: 0;
            left: 0;
            background-color: rgba(255, 255, 255, 0);
            transition: background-color 0.4s ease;
            z-index: 1000;
        }
        #main-header.scrolled {
            background-color: rgba(255, 255, 255, 0.7);
        }
        #main-header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        #main-header h1 {
            font-size: 1.5rem;
            color: #f0f3f5;
        }
        #main-header nav ul {
            display: flex;
            list-style: none;
        }
        #main-header nav ul li {
            margin-right: 20px;
        }
        #main-header nav ul li a {
            color: #f0f3f5;
            text-decoration: none;
            font-weight: bold;
        }
        .newsletter-btn {
            background-color: rgb(0, 156, 223);
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            font-weight: bold;
        }
        /* Ajustes generales para el contenedor principal */
        #main-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 100px;
            /* Para evitar que el contenido quede bajo el header fijo */
            padding-bottom: 50px;
        }
        .text-content {
            width: 55%;
        }
        .text-content h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        .text-content span {
            color: rgb(0, 156, 223);
        }
        .text-content p {
            margin-bottom: 15px;
        }
        .text-content2 {
            width: 55%;
        }
        .text-content2 h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: rgb(0, 38, 77);
        }
        .text-content2 span {
            color: rgb(0, 156, 223);
        }
        .image-content {
            width: 35%;
            margin-left: 20px;
            display: flex;
        }
        .image-content img {
            max-width: 70%;
            border-radius: 10px;
            object-fit: cover;
            height: auto;
        }
        /* Sección de la galería (timeline) */
        #timeline {
            background-color: #ffffff;
            padding: 50px 0;
            position: relative;
        }
        .gallery {
            display: flex;
            overflow-x: auto;
            scroll-behavior: smooth;
        }
        .gallery img {
            width: 500px;
            flex-shrink: 0;
            border-radius: 10px;
        }
        .gallery img+img {
            margin-left: -5px;
            /* Elimina los espacios entre imágenes */
        }
        /* Formación Académica */
        #Formacion {
            background-color: rgb(4, 31, 59);
            padding: 50px 0;
            position: relative;
        }
        /* Estilos para el carrusel */
        .carousel {
            position: relative;
            max-width: 600px;
            margin: 40px auto;
            overflow: hidden;
        }
        .carousel-inner {
            display: flex;
            transition: transform 0.5s ease-in-out;
        }
        .carousel-item {
            min-width: 100%;
            text-align: center;
        }
        .carousel-item img {
            width: 100%;
            height: 300px;
            object-fit: contain;
            border-radius: 10px;
            background-color: #f0f0f0;
        }
        .carousel-item p {
            margin-top: 10px;
            color: #f0f3f5;
            font-size: 1rem;
        }
        /* Botones del carrusel */
        .prev-btn,
        .next-btn {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(0, 0, 0, 0.5);
            border: none;
            color: white;
            padding: 10px;
            cursor: pointer;
        }
        .prev-btn {
            left: 10px;
        }
        .next-btn {
            right: 10px;
        }
        .prev-btn:hover,
        .next-btn:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }
        /* Footer */
        footer {
            background-color: #002244;
            color: white;
            text-align: center;
            font-size: small;
            font-style: italic;
            padding: 20px 0;
        }
        /* Responsivo */
        @media (max-width: 768px) {
            #main-content {
                flex-direction: column;
                text-align: center;
            }
            .text-content,
            .image-content {
                width: 100%;
            }
            .text-content h2 {
                font-size: 2rem;
            }
            .text-content p {
                font-size: 1rem;
            }
            .gallery img {
                width: 80%;
            }
        }
    </style>
</head>

<body>
    <!-- Encabezado -->
    <header id="main-header">
        <div class="container">
            <div class="logo">
                <h1>Victor Cercado</h1>
            </div>
            <nav>
                <ul>
                    <li><a href="#">Biografía</a></li>
                    <li><a href="#">Mis Proyectos</a></li>
                    <li><a href="#">Opinión Bursátil</a></li>
                    <li><a href="#">Contáctame</a></li>
                    <li><a href="#">Otro</a></li>
                </ul>
            </nav>
            <button class="newsletter-btn">NEWSLETTER</button>
        </div>
    </header>
    <!-- Contenido principal -->
    <section id="main-content">
        <div class="container">
            <div class="text-content">
                <h2>Economista, <span>apasionado por los mercados financieros</span> y la tecnología</h2>
                <p>Soy economista con experiencia en el análisis de mercados financieros y una gran pasión 
                    por la tecnología. Estoy comprometido con el aprendizaje continuo y el desarrollo de 
                    soluciones innovadoras para el sector financiero. </p>
                <p>Tengo un especial interés en el uso de herramientas como VBA, Power BI y Python para
                    la automatización de procesos y el análisis de datos. Actualmente, estoy desarrollando 
                    habilidades para la creación de aplicaciones web que resuelvan problemas o mejoren
                     la experiencia del usuario.</p>
            </div>
            <div class="image-content">
                <img src="ZIMG-2022.jpg" alt="Foto de Victor Cercado">
            </div>
        </div>
    </section>
    <!-- Sección de galería (timeline) -->
    <section id="timeline">
        <div class="container2">
            <div class="text-content2">
                <h2>Experiencia <span>Laboral</span></h2>
            </div>
            <div class="gallery">
                <img src="1.png" alt="Imagen 1">
                <img src="2.png" alt="Imagen 2">
                <img src="3.png" alt="Imagen 3">
            </div>
       </div>
    </section>
    <!-- Sección de Formación Académica -->
    <section id="Formacion">
        <div class="container2">
            <div class="text-content">
                <h2>Formación <span>Académica</span></h2>
            </div>
            <div class="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <img src="BCRP.png" alt="BCRP_img">
                        <p>Becario Curso de Extensión en Finanzas Avanzadas - BCRP</p>
                    </div>
                    <div class="carousel-item">
                        <img src="PEMV.png" alt="SMV_img">
                        <p>Becario Programa de Especialización en Mercado de Valores - SMV</p>
                    </div>
                    <div class="carousel-item">
                        <img src="estudio3.jpg" alt="UNTRM_img">
                        <p>Licenciado en Economía - UNTRM</p>
                    </div>
                </div>
                <button class="prev-btn">❮</button>
                <button class="next-btn">❯</button>
            </div>
        </div>
    </section>
    <footer>
        <p>&copy; 2024 Victor Cercado. Todos los derechos reservados.</p>
    </footer>
</body>
</html>
<script>
    // Cambiar el fondo del encabezado al hacer scroll
    window.addEventListener('scroll', function () {
        const header = document.getElementById('main-header');
        if (window.scrollY > 50) {
            header.classList.add('scrolled');
        } else {
            header.classList.remove('scrolled');
        }
    });
    // Funcionalidad del carrusel
    let currentSlide = 0;
    const slides = document.querySelectorAll('.carousel-item');
    const totalSlides = slides.length;
    document.querySelector('.next-btn').addEventListener('click', () => {
        currentSlide = (currentSlide + 1) % totalSlides;
        updateCarousel();
    });
    document.querySelector('.prev-btn').addEventListener('click', () => {
        currentSlide = (currentSlide - 1 + totalSlides) % totalSlides;
        updateCarousel();
    });
    function updateCarousel() {
        const offset = -currentSlide * 100;
        document.querySelector('.carousel-inner').style.transform = `translateX(${offset}%)`;
    }
</script>


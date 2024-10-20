/* Estilos generales */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    line-height: 1.6;
    color: #333;
    background-color: #f4f4f4;
}

/* Contenedor */
.container {
    width: 80%;
    margin: auto;
    overflow: hidden;
}

/* Encabezado principal */
.main-header {
    background-color: #003366;
    color: #fff;
    padding: 30px 0;
    text-align: center;
}

.main-header h1 {
    font-size: 2.5rem;
    margin-bottom: 10px;
}

.main-header p {
    font-size: 1.2rem;
}

.main-header img {
    width: 150px;
    border-radius: 50%;
    margin-top: 20px;
}

/* Sección de servicios */
.services-section {
    background-color: #fff;
    padding: 30px 0;
}

.services-grid {
    display: flex;
    justify-content: space-between;
}

.service {
    text-align: center;
    width: 30%;
}

.service img {
    width: 80px;
    margin-bottom: 15px;
}

/* Sección de testimonios */
.testimonials-section {
    background-color: #e6f7ff;
    padding: 30px 0;
    text-align: center;
}

.testimonial {
    margin-bottom: 20px;
}

.testimonial p {
    font-style: italic;
}

/* Sección del blog */
.blog-section {
    background-color: #fff;
    padding: 30px 0;
}

.blog-post {
    margin-bottom: 20px;
}

.blog-post h3 {
    color: #003366;
}

/* Sección de contacto */
.contact-section {
    background-color: #003366;
    color: #fff;
    padding: 30px 0;
    text-align: center;
}

.contact-form input, 
.contact-form textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
}

button {
    padding: 10px 20px;
    background-color: #0066cc;
    color: white;
    border: none;
    cursor: pointer;
}

button:hover {
    background-color: #00509e;
}

/* Footer */
footer {
    background-color: #002244;
    color: white;
    text-align: center;
    padding: 20px 0;
}

/* Responsivo */
@media (max-width: 768px) {
    .services-grid {
        flex-direction: column;
        text-align: center;
    }

    .service {
        width: 100%;
        margin-bottom: 20px;
    }
}
/* Add styles here */







<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Impulsando el Crecimiento Financiero</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Página de inicio -->
    <header class="main-header">
        <div class="container">
            <h1>Impulsando el Crecimiento Financiero</h1>
            <p>Bienvenido a mi sitio web. Con una sólida experiencia en mercados financieros, mi objetivo es ayudarte a alcanzar tus metas de inversión.</p>
            <img src="ZIMG-2022.jpg" alt="FotoPerfil">
        </div>
    </header>

    <!-- Sección de servicios -->
    <section id="services" class="services-section">
        <div class="container">
            <h2>Mis Servicios</h2>
            <div class="services-grid">
                <div class="service">
                    <img src="icono-inversiones.png" alt="Asesoría en Inversiones">
                    <h3>Asesoría en Inversiones</h3>
                    <p>Te ayudo a tomar decisiones informadas para optimizar tus inversiones.</p>
                </div>
                <div class="service">
                    <img src="icono-portafolio.png" alt="Gestión de Portafolios">
                    <h3>Gestión de Portafolios</h3>
                    <p>Gestiono tu portafolio de manera estratégica para maximizar tu rentabilidad.</p>
                </div>
                <div class="service">
                    <img src="icono-consultoria.png" alt="Consultoría Financiera">
                    <h3>Consultoría Financiera</h3>
                    <p>Te ofrezco análisis detallado del mercado y estrategias financieras personalizadas.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonios -->
    <section id="testimonials" class="testimonials-section">
        <div class="container">
            <h2>Testimonios de Clientes</h2>
            <div class="testimonial">
                <p>"Gracias a la asesoría, logré un crecimiento significativo en mi portafolio. Altamente recomendable."</p>
                <p><strong>- Juan Pérez, CEO de Empresa X</strong></p>
            </div>
            <div class="testimonial">
                <p>"La mejor experiencia trabajando con un profesional en mercados financieros. Me ayudó a diversificar mis inversiones."</p>
                <p><strong>- Ana García, Inversora</strong></p>
            </div>
        </div>
    </section>

    <!-- Casos de estudio / Blog -->
    <section id="blog" class="blog-section">
        <div class="container">
            <h2>Artículos y Casos de Estudio</h2>
            <div class="blog-posts">
                <article class="blog-post">
                    <h3>Análisis del Mercado Actual</h3>
                    <p>En este artículo, exploro las tendencias más recientes en los mercados financieros...</p>
                    <a href="#">Leer más</a>
                </article>
                <article class="blog-post">
                    <h3>Estrategias de Diversificación</h3>
                    <p>Descubre cómo diversificar tu portafolio para minimizar riesgos y optimizar rendimientos...</p>
                    <a href="#">Leer más</a>
                </article>
            </div>
        </div>
    </section>

    <!-- Página de contacto -->
    <section id="contact" class="contact-section">
        <div class="container">
            <h2>Contacto</h2>
            <form id="contact-form">
                <label for="name">Nombre</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Correo Electrónico</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Mensaje</label>
                <textarea id="message" name="message" required></textarea>

                <button type="submit">Enviar</button>
            </form>
            <div class="social-links">
                <a href="https://www.linkedin.com/in/tu-perfil/">LinkedIn</a>
                <a href="mailto:tu-email@gmail.com">Correo</a>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Impulsando el Crecimiento Financiero. Todos los derechos reservados.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>







// Script básico para validar el formulario de contacto
document.getElementById('contact-form').addEventListener('submit', function(event) {
    event.preventDefault();
    alert('Gracias por tu mensaje. Nos pondremos en contacto contigo pronto.');
});

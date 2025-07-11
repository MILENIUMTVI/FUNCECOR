<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Luz de la Fe: Fortaleciendo Familias con Valores Católicos, un proyecto de FUNCECOR que usa medios de comunicación para difundir fe, esperanza y amor.">
    <meta name="keywords" content="valores católicos, fe, esperanza, caridad, familia, comunidad, FUNCECOR, medios católicos, educación espiritual">
    <meta name="author" content="FUNCECOR">
    <meta name="robots" content="index, follow">
    <title>Luz de la Fe - FUNCECOR</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&family=Lora:wght@400;700&family=Cormorant+Garamond:wght@400;700&family=Montserrat:wght@500;600&display=swap" rel="stylesheet">
    <!-- Font Awesome para íconos -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(135deg, #f0f4f8, #e0e8f0, #d6e6f2);
            color: #333;
            line-height: 1.6;
            overflow-x: hidden;
            font-size: 16px;
        }

        /* Encabezado */
        header {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('banner.jpg');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 6rem 1rem;
            position: relative;
            animation: fadeInDown 2s ease-out;
        }

        header .header-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            gap: 1.5rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        header h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: clamp(2.5rem, 8vw, 4rem);
            margin: 0;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
            letter-spacing: 2px;
        }

        header img.logo {
            max-width: min(250px, 40vw);
            height: auto;
            transition: transform 0.5s ease, box-shadow 0.5s ease;
        }

        header img.logo:hover {
            transform: scale(1.1);
            box-shadow: 0 0 15px rgba(255,215,0,0.6);
        }

        header p {
            font-size: clamp(1rem, 3vw, 1.3rem);
            max-width: 800px;
            margin: 1.5rem auto 0;
            font-family: 'Montserrat', sans-serif;
            opacity: 0.95;
        }

        /* Animaciones */
        @keyframes fadeInDown {
            from { opacity: 0; transform: translateY(-40px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Navegación */
        nav {
            background: linear-gradient(90deg, #1a5f7a, #0f3c4c, #0a2a36);
            padding: 1rem;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }

        nav ul {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            list-style: none;
            gap: 1.5rem;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-family: 'Montserrat', sans-serif;
            font-size: clamp(0.9rem, 2.5vw, 1.1rem);
            transition: color 0.3s, text-shadow 0.3s;
        }

        nav ul li a:hover {
            color: #ffd700;
            text-shadow: 0 0 10px rgba(255,215,0,0.8);
        }

        /* Contenedor Principal */
        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 2rem 1rem;
        }

        /* Sección Hero */
        .hero {
            text-align: center;
            padding: 4rem 1rem;
            background: linear-gradient(135deg, #ffffff, #f0f4f8, #e0e8f0);
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
            margin-bottom: 3rem;
            animation: slideUpFade 2s ease-out;
        }

        .hero h2 {
            font-family: 'Cormorant Garamond', serif;
            color: #1a5f7a;
            font-size: clamp(2rem, 6vw, 3rem);
            margin-bottom: 1.5rem;
            letter-spacing: 1px;
        }

        .hero p {
            font-size: clamp(1rem, 3vw, 1.2rem);
            max-width: 900px;
            margin: 0 auto 2rem;
            color: #444;
            font-family: 'Lora', serif;
        }

        .multimedia {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .multimedia iframe, .multimedia audio {
            width: 100%;
            max-width: 600px;
            border-radius: 10px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .multimedia iframe:hover, .multimedia audio:hover {
            transform: scale(1.02);
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
        }

        /* Animación */
        @keyframes slideUpFade {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        /* Secciones Generales */
        .section {
            background: linear-gradient(135deg, #ffffff, #f8fafc, #f0f4f8);
            padding: 3rem 1.5rem;
            margin-bottom: 3rem;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
            transition: transform 0.4s ease, box-shadow 0.4s ease;
        }

        .section:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 25px rgba(0,0,0,0.15);
        }

        .section h2 {
            font-family: 'Cormorant Garamond', serif;
            color: #1a5f7a;
            font-size: clamp(1.8rem, 5vw, 2.5rem);
            margin-bottom: 1.5rem;
            text-align: center;
        }

        .section p {
            font-size: clamp(0.95rem, 2.5vw, 1.1rem);
            color: #555;
            line-height: 1.8;
            margin-bottom: 1.5rem;
        }

        .section ul {
            list-style: none;
            margin-left: 1.5rem;
        }

        .section ul li {
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            margin-bottom: 0.8rem;
            position: relative;
        }

        .section ul li:before {
            content: "✝";
            color: #1a5f7a;
            position: absolute;
            left: -1.2rem;
        }

        /* Testimonios */
        .testimonials {
            background: linear-gradient(135deg, #e8f1f2, #d6e6f2, #c0d6e4);
            padding: 3rem 1.5rem;
            border-radius: 15px;
            margin-bottom: 3rem;
        }

        .testimonial {
            margin-bottom: 2rem;
            font-style: italic;
            font-size: clamp(0.95rem, 2.5vw, 1.1rem);
            color: #333;
            padding: 1.5rem;
            background: linear-gradient(135deg, #ffffff, #f8fafc);
            border-radius: 10px;
            box-shadow: 0 6px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .testimonial:hover {
            transform: translateY(-5px);
        }

        /* Formulario */
        .contact-form {
            display: flex;
            flex-direction: column;
            gap: 1.2rem;
            max-width: 700px;
            margin: 0 auto;
            padding: 2rem;
            background: linear-gradient(135deg, #ffffff, #f0f4f8);
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
        }

        .contact-form input, .contact-form textarea {
            padding: 1rem;
            border: 1px solid #ccc;
            border-radius: 8px;
            font-size: clamp(0.9rem, 2.5vw, 1rem);
            transition: border-color 0.3s, box-shadow 0.3s;
        }

        .contact-form input:focus, .contact-form textarea:focus {
            border-color: #1a5f7a;
            box-shadow: 0 0 10px rgba(26,95,122,0.3);
            outline: none;
        }

        .contact-form button {
            background: linear-gradient(135deg, #1a5f7a, #0f3c4c);
            color: white;
            padding: 1rem;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: clamp(0.9rem, 2.5vw, 1.1rem);
            font-weight: 600;
            text-transform: uppercase;
            transition: background 0.3s, transform 0.3s, box-shadow 0.3s;
        }

        .contact-form button:hover {
            background: linear-gradient(135deg, #0f3c4c, #1a5f7a);
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0,0,0,0.2);
        }

        /* Pie de Página */
        footer {
            background: linear-gradient(135deg, #1a5f7a, #0f3c4c, #0a2a36);
            color: white;
            text-align: center;
            padding: 2rem 1rem;
            margin-top: 3rem;
        }

        footer a {
            color: #ffd700;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s, text-shadow 0.3s;
        }

        footer a:hover {
            color: #ffeb3b;
            text-shadow: 0 0 10px rgba(255,235,59,0.8);
        }

        footer p {
            font-size: clamp(0.85rem, 2.5vw, 1rem);
            margin-bottom: 0.5rem;
        }

        /* Responsividad */
        @media (min-width: 768px) {
            header .header-content {
                flex-direction: row;
                gap: 2rem;
            }

            nav ul {
                flex-wrap: nowrap;
            }
        }

        @media (max-width: 768px) {
            header {
                padding: 4rem 1rem;
            }

            header h1 {
                font-size: clamp(2rem, 7vw, 3rem);
            }

            header img.logo {
                max-width: min(200px, 50vw);
            }

            nav ul {
                flex-direction: column;
                gap: 1rem;
                text-align: center;
            }

            .hero {
                padding: 3rem 1rem;
            }

            .hero h2 {
                font-size: clamp(1.8rem, 6vw, 2.5rem);
            }

            .multimedia {
                grid-template-columns: 1fr;
            }

            .section {
                padding: 2rem 1rem;
            }

            .contact-form {
                padding: 1.5rem;
            }
        }

        @media (max-width: 480px) {
            body {
                font-size: 14px;
            }

            header {
                padding: 3rem 0.5rem;
            }

            header p {
                padding: 0 1rem;
            }

            .hero {
                padding: 2rem 0.5rem;
            }

            .section h2 {
                font-size: clamp(1.5rem, 5vw, 2rem);
            }

            .contact-form input, .contact-form textarea, .contact-form button {
                font-size: clamp(0.85rem, 2.5vw, 0.95rem);
            }
        }
    </style>
</head>
<body>
    <!-- Encabezado -->
    <header role="banner">
        <div class="header-content">
            <img src="logo.png" alt="Logo FUNCECOR - Fundación Educativa para el Desarrollo" class="logo">
            <h1>FUNCECOR</h1>
        </div>
        <p>Luz de la Fe: Un faro que ilumina el camino de las familias católicas, fortaleciendo su fe, amor y unidad en un mundo de desafíos modernos.</p>
    </header>

    <!-- Navegación -->
    <nav role="navigation">
        <ul>
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#resumen">Resumen</a></li>
            <li><a href="#objetivos">Objetivos</a></li>
            <li><a href="#justificacion">Justificación</a></li>
            <li><a href="#publico">Público</a></li>
            <li><a href="#estrategias">Estrategias</a></li>
            <li><a href="#plan">Plan</a></li>
            <li><a href="#recursos">Recursos</a></li>
            <li><a href="#indicadores">Indicadores</a></li>
            <li><a href="#riesgos">Riesgos</a></li>
            <li><a href="#conclusion">Conclusión</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
    </nav>

    <!-- Contenedor Principal -->
    <main class="container" role="main">
        <!-- Sección Hero -->
        <section id="inicio" class="hero" aria-labelledby="hero-title">
            <h2 id="hero-title">Luz de la Fe: Fortaleciendo Familias</h2>
            <p>Bienvenidos a un proyecto transformador de FUNCECOR que utiliza los medios de comunicación para difundir los valores católicos, inspirando a las familias a vivir su fe con alegría y compromiso en un mundo cambiante.</p>
            <div class="multimedia">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/zoKoxeSRIag" title="Introducción a Luz de la Fe" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </section>

        <!-- Sección Resumen Ejecutivo -->
        <section id="resumen" class="section" aria-labelledby="resumen-title">
            <h2 id="resumen-title">Resumen Ejecutivo</h2>
            <p>El proyecto <strong>"Luz de la Fe"</strong> busca promover los valores católicos en las familias mediante una estrategia integral de medios de comunicación. En un mundo donde las familias enfrentan desafíos culturales, sociales y tecnológicos, este proyecto utiliza plataformas digitales, radio, televisión y eventos comunitarios para difundir mensajes que refuercen la fe, el amor, la unidad y la moral cristiana, inspirando a las familias a ser el núcleo vivo de la sociedad.</p>
        </section>

        <!-- Sección Objetivos -->
        <section id="objetivos" class="section" aria-labelledby="objetivos-title">
            <h2 id="objetivos-title">Objetivos</h2>
            <p><strong>General:</strong> Difundir los valores católicos (fe, esperanza, caridad, respeto, responsabilidad, perdón y solidaridad) para fortalecer la vida familiar y su impacto en la comunidad.</p>
            <p><strong>Específicos:</strong></p>
            <ul>
                <li>Crear contenido multimedia atractivo que conecte con familias de diferentes edades y contextos.</li>
                <li>Fomentar la participación activa de las familias en actividades que refuercen los valores cristianos.</li>
                <li>Establecer una red de medios de comunicación católica que sea accesible y sostenible.</li>
                <li>Promover el diálogo intergeneracional sobre la fe y los valores en el hogar.</li>
            </ul>
        </section>

        <!-- Sección Justificación -->
        <section id="justificacion" class="section" aria-labelledby="justificacion-title">
            <h2 id="justificacion-title">Justificación</h2>
            <p>La familia, según el Catecismo de la Iglesia Católica (2207), es la base de la sociedad. Hoy, enfrenta retos como la secularización, la influencia de medios contrarios a la fe y la falta de tiempo para la convivencia y la oración. "Luz de la Fe" responde a esta necesidad con contenido inspirador que invita a las familias a vivir su fe con alegría y compromiso, utilizando medios modernos para alcanzar a un público amplio y diverso.</p>
        </section>

        <!-- Sección Público Objetivo -->
        <section id="publico" class="section" aria-labelledby="publico-title">
            <h2 id="publico-title">Público Objetivo</h2>
            <p><strong>Primario:</strong> Familias católicas de habla castellana, con énfasis en padres de familia (25-50 años) y niños/jóvenes (5-18 años).</p>
            <p><strong>Secundario:</strong> Líderes comunitarios, educadores católicos y parroquias interesadas en promover valores cristianos.</p>
            <p><strong>Alcance Geográfico:</strong> Inicialmente en las provincias de Azuay y Cañar, con planes de expansión.</p>
        </section>

        <!-- Sección Estrategias de Comunicación -->
        <section id="estrategias" class="section" aria-labelledby="estrategias-title">
            <h2 id="estrategias-title">Estrategias de Comunicación</h2>
            <h3>Contenidos Multimedia</h3>
            <ul>
                <li><strong>Videos:</strong> Series cortas como "Historias de Fe" (3 minutos) en YouTube, Instagram y TikTok, usando IPTV Milenium TVi.</li>
                <li><strong>Podcasts:</strong> "Familia en Oración", un programa semanal con reflexiones del Evangelio y consejos familiares.</li>
                <li><strong>Redes Sociales:</strong> Publicaciones diarias con frases, retos como "Día de oración en familia" y lives con sacerdotes.</li>
                <li><strong>Aplicación Móvil:</strong> App con guías de oración, catequesis y calendario litúrgico.</li>
            </ul>
            <h3>Televisión y Radio</h3>
            <ul>
                <li><strong>TV:</strong> "Hogar de Luz" semanal en ACADEMIA, con dinámicas familiares.</li>
                <li><strong>Radio:</strong> Segmentos de 5 minutos en Ondas Cañaris y Radio Catedral.</li>
            </ul>
            <h3>Eventos Comunitarios</h3>
            <ul>
                <li><strong>Jornadas Familiares:</strong> Talleres y actividades parroquiales.</li>
                <li><strong>Campañas Anuales:</strong> "Mes de la Familia Cristiana" con oración y valores.</li>
            </ul>
            <h3>Material Impreso y Digital</h3>
            <ul>
                <li>Folletos y guías descargables para oración y actividades.</li>
                <li>Revista digital mensual sobre educación en la fe.</li>
            </ul>
        </section>

        <!-- Sección Plan de Acción -->
        <section id="plan" class="section" aria-labelledby="plan-title">
            <h2 id="plan-title">Plan de Acción</h2>
            <h3>Fase 1: Investigación y Planeación (Meses 1-3)</h3>
            <ul>
                <li>Diagnóstico mediante encuestas en parroquias y redes sociales.</li>
                <li>Formación de un equipo con expertos en comunicación y teología.</li>
                <li>Diseño de identidad visual y narrativa.</li>
            </ul>
            <h3>Fase 2: Producción de Contenidos (Meses 4-9)</h3>
            <ul>
                <li>Grabación de videos y podcasts iniciales.</li>
                <li>Creación de contenido para redes y la app.</li>
                <li>Coordinación con canales y emisoras.</li>
            </ul>
            <h3>Fase 3: Lanzamiento y Difusión (Meses 10-12)</h3>
            <ul>
                <li>Campaña con evento virtual.</li>
                <li>Jornadas familiares en parroquias piloto.</li>
                <li>Monitoreo de retroalimentación.</li>
            </ul>
            <h3>Fase 4: Evaluación y Expansión (Año 2)</h3>
            <ul>
                <li>Análisis de métricas de audiencia.</li>
                <li>Ajustes según retroalimentación.</li>
                <li>Expansión a nuevas regiones.</li>
            </ul>
        </section>

        <!-- Sección Recursos Necesarios -->
        <section id="recursos" class="section" aria-labelledby="recursos-title">
            <h2 id="recursos-title">Recursos Necesarios</h2>
            <ul>
                <li><strong>Humanos:</strong> Periodistas, productores, teólogos, sacerdotes y voluntarios.</li>
                <li><strong>Técnicos:</strong> Equipos de grabación, software y hosting.</li>
                <li><strong>Financieros:</strong> $10,000 USD iniciales vía donaciones y crowdfunding.</li>
                <li><strong>Alianzas:</strong> Diócesis, Radio Catedral, Radio María.</li>
            </ul>
        </section>

        <!-- Sección Indicadores de Éxito -->
        <section id="indicadores" class="section" aria-labelledby="indicadores-title">
            <h2 id="indicadores-title">Indicadores de Éxito</h2>
            <p><strong>Cuantitativos:</strong></p>
            <ul>
                <li>1,000 suscriptores en YouTube y 1,000 seguidores en redes en el primer año.</li>
                <li>100 descargas de la app en 6 meses.</li>
                <li>2 jornadas familiares con 50 asistentes cada una.</li>
            </ul>
            <p><strong>Cualitativos:</strong></p>
            <ul>
                <li>Retroalimentación positiva sobre impacto espiritual.</li>
                <li>Testimonios de cambios familiares (oración, diálogo).</li>
                <li>Incremento en participación parroquial.</li>
            </ul>
        </section>

        <!-- Sección Riesgos y Mitigación -->
        <section id="riesgos" class="section" aria-labelledby="riesgos-title">
            <h2 id="riesgos-title">Riesgos y Mitigación</h2>
            <ul>
                <li><strong>Falta de interés:</strong> Crear contenido dinámico con pruebas piloto.</li>
                <li><strong>Limitaciones presupuestarias:</strong> Financiamiento diversificado y priorización de bajo costo.</li>
                <li><strong>Resistencia cultural:</strong> Mensajes inclusivos enfocados en amor y unidad.</li>
            </ul>
        </section>

        <!-- Sección Conclusión -->
        <section id="conclusion" class="section" aria-labelledby="conclusion-title">
            <h2 id="conclusion-title">Conclusión</h2>
            <p>"Luz de la Fe" es un proyecto ambicioso y esencial para revitalizar la vivencia de los valores católicos en las familias. Con una estrategia multimedia y comunitaria, no solo difundimos la fe, sino que inspiramos a las familias a ser testigos vivos del amor de Cristo. Con el respaldo de la comunidad católica y una planificación rigurosa, este proyecto será un faro de esperanza para generaciones presentes y futuras.</p>
        </section>

        <!-- Sección Contacto -->
        <section id="contacto" class="section" aria-labelledby="contacto-title">
            <h2 id="contacto-title">Contáctanos</h2>
            <p>Únete a esta misión de fe. Compártenos tus ideas, sugerencias o peticiones de oración para fortalecer nuestra comunidad de fe.</p>
            <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
                <input type="text" name="name" placeholder="Tu Nombre Completo" required aria-label="Nombre">
                <input type="email" name="email" placeholder="Tu Correo Electrónico" required aria-label="Correo Electrónico">
                <textarea name="message" placeholder="Tu Mensaje o Petición de Oración" rows="8" required aria-label="Mensaje"></textarea>
                <button type="submit">Enviar con Fe</button>
            </form>
        </section>
    </main>

    <!-- Pie de Página -->
    <footer role="contentinfo">
        <p>© 2025 FUNCECOR - Luz de la Fe. Todos los derechos reservados.</p>
        <p>Síguenos en <a href="https://facebook.com/funcecor" target="_blank"><i class="fab fa-facebook"></i> Facebook</a> | <a href="https://instagram.com/funcecor" target="_blank"><i class="fab fa-instagram"></i> Instagram</a> | <a href="mailto:contacto@funcecor.org">contacto@funcecor.org</a></p>
        <p>Creado con devoción para la gloria de Dios y el bien de las familias.</p>
    </footer>
</body>
</html>

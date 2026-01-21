# eskubilbot
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EskuBilbot | UPV/EHU Robotic Arm Project</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --magenta-oficial: #e2007a;
            --magenta-oscuro: #b0005f;
            --blanco: #ffffff;
            --gris-claro: #f4f4f4;
            --negro-texto: #1a1a1a;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', sans-serif;
        }

        body {
            line-height: 1.6;
            color: var(--negro-texto);
            background-color: var(--blanco);
        }

        /* --- NAVEGACIÓN --- */
        nav {
            background: var(--blanco);
            padding: 1rem 5%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-weight: 700;
            font-size: 1.5rem;
            color: var(--magenta-oficial);
            text-decoration: none;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--negro-texto);
            font-weight: 500;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--magenta-oficial);
        }

        /* --- HERO / PROYECTO --- */
        header {
            height: 80vh;
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1581091226825-a6a2a5aee158?auto=format&fit=crop&q=80') center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
            padding: 0 20px;
            margin-top: 60px;
        }

        header h1 { font-size: 3.5rem; margin-bottom: 1rem; }
        header p { font-size: 1.2rem; max-width: 800px; }

        section { padding: 80px 10% 40px; }
        h2 {
            color: var(--magenta-oficial);
            font-size: 2.5rem;
            margin-bottom: 2rem;
            text-align: center;
            border-bottom: 3px solid var(--magenta-oficial);
            display: inline-block;
            left: 50%;
            transform: translateX(-50%);
            position: relative;
        }

        .grid-info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .card {
            background: var(--gris-claro);
            padding: 2rem;
            border-radius: 10px;
            border-left: 5px solid var(--magenta-oficial);
        }

        /* --- EQUIPO --- */
        .equipo-container {
            margin-bottom: 4rem;
        }

        h3 { color: var(--magenta-oscuro); margin: 1.5rem 0; font-size: 1.8rem; }

        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }

        .member-card {
            background: white;
            border: 1px solid #ddd;
            padding: 15px;
            text-align: center;
            border-radius: 8px;
            transition: transform 0.3s;
        }

        .member-card:hover { transform: translateY(-5px); box-shadow: 0 5px 15px rgba(0,0,0,0.1); }

        .member-photo {
            width: 100px;
            height: 100px;
            background: #ccc;
            border-radius: 50%;
            margin: 0 auto 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }

        .member-photo img { width: 100%; height: 100%; object-fit: cover; }

        /* --- PATROCINADORES --- */
        .sponsors-grid {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 40px;
            align-items: center;
            opacity: 0.7;
        }

        .sponsor-placeholder {
            width: 150px;
            height: 80px;
            border: 2px dashed #ccc;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.8rem;
            color: #999;
        }

        footer {
            background: var(--negro-texto);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 40px;
        }

        .btn {
            background: var(--magenta-oficial);
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            display: inline-block;
            margin-top: 10px;
        }

    </style>
</head>
<body>

    <nav>
        <a href="#" class="logo">ESKUBILBOT</a>
        <ul>
            <li><a href="#proyecto">Proyecto</a></li>
            <li><a href="#equipo">Equipo</a></li>
            <li><a href="#patrocinadores">Patrocinadores</a></li>
        </ul>
    </nav>

    <header id="proyecto">
        <h1>EskuBilbot</h1>
        <p>Innovación en biónica y robótica desde la UPV/EHU para la II Competición Universitaria de Mano Protésicas.</p>
        <a href="https://sites.google.com/uji.es/icompeticionprotesismano/inicio" class="btn" target="_blank">Ver Competición</a>
    </header>

    <section>
        <h2>El Proyecto</h2>
        <div class="grid-info">
            <div class="card">
                <h3>¿Quiénes Somos?</h3>
                <p>Un equipo multidisciplinar de estudiantes de la Universidad del País Vasco (UPV/EHU) apasionados por la tecnología asistiva y la ingeniería.</p>
            </div>
            <div class="card">
                <h3>¿Qué es EskuBilbot?</h3>
                <p>Es un proyecto universitario challenge based learning</p>
            </div>
            <div class="card">
                <h3>¿Qué hacemos?</h3>
                <p>Diseñamos, fabricamos y programamos una prótesis completa capaz de realizar tareas cotidianas complejas mediante control mioeléctrico y sensores avanzados.</p>
            </div>
            <div class="card">
                <h3>La Competición</h3>
                <p>Participamos en la <strong>Valencia 2026</strong>, basada en los estándares de <em>Cybathlon</em>, donde nuestra prótesis será puesta a prueba en velocidad y precisión.</p>
            </div>
        </div>
    </section>

    <hr>

    <section id="equipo">
        <h2>Nuestro Equipo</h2>

        <div class="equipo-container">
            <h3>El Piloto</h3>
            <div class="team-grid">
                <div class="member-card">
                    <div class="member-photo">👤
                    </div>
                    <strong>Nombre del Piloto</strong>
                    <p>Atleta Cybathlon</p>
                </div>
            </div>
        </div>

        <div class="equipo-container">
            <h3>Profesores Guía</h3>
            <div class="team-grid">
                <div class="member-card">
                    <div class="member-photo">🎓</div>
                    <strong>Nombre Profesor</strong>
                    <p>Mentor Académico</p>
                </div>
                </div>
        </div>

        <div class="equipo-container">
            <h3>Grupos de Trabajo</h3>
           
            <h4>1. Biomecánica</h4>
            <p style="margin-bottom:1rem;">Análisis de pruebas, diseño de interfaz humano-protésica y ergonomía.</p>
            <div class="team-grid">
                <div class="member-card"><strong>Estudiante A</strong></div>
                <div class="member-card"><strong>Estudiante B</strong></div>
            </div>

            <h4 style="margin-top:2rem;">2. Control y Automática</h4>
            <p style="margin-bottom:1rem;">Integración de sensores, actuadores y lógica de programación.</p>
            <div class="team-grid">
                <div class="member-card"><strong>Estudiante C</strong></div>
                <div class="member-card"><strong>Estudiante D</strong></div>
            </div>

            <h4 style="margin-top:2rem;">3. Diseño Mecánico</h4>
            <p style="margin-bottom:1rem;">Modelado CAD, selección de materiales biocompatibles y fabricación.</p>
            <div class="team-grid">
                <div class="member-card"><strong>Estudiante E</strong></div>
                <div class="member-card"><strong>Estudiante F</strong></div>
            </div>
        </div>
    </section>

    <section id="patrocinadores" style="background: var(--gris-claro); text-align: center;">
        <h2>Patrocinadores</h2>
        <p>¿Quieres apoyar el desarrollo de tecnología biónica local? Únete a nosotros.</p>
        <br><br>
        <div class="sponsors-grid">
            <div class="sponsor-placeholder">Espacio disponible</div>
            <div class="sponsor-placeholder">Espacio disponible</div>
            <div class="sponsor-placeholder">Espacio disponible</div>
        </div>
        <br>
        <a href="mailto:tuemail@ehu.eus" class="btn">Convertirse en Patrocinador</a>
    </section>

    <footer>
        <p>&copy; 2026 EskuBilbot - Proyecto Universitario UPV/EHU</p>
    </footer>

</body>
</html>


# Inrrigacion-santa-rosa-
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Irrigación Santa Rosa – La Villa | Identidad, Agricultura y Sostenibilidad</title>
    <meta name="description" content="Portal oficial de Irrigación Santa Rosa - La Villa. Historia, educación cívica, agricultura tecnificada, tradiciones y desarrollo comunitario sostenible.">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        /* ==========================================================================
           1. VARIABLES Y DISEÑO DEL SISTEMA DE COLOR (Blanco, Crema, Verde Limón, Verde Oscuro, Azul)
           ========================================================================== */
        :root {
            --color-cream: #faf6f0;        /* Crema base */
            --color-cream-light: #fdfbf7;  /* Crema muy suave */
            --color-white: #ffffff;
            --color-dark-green: #143625;   /* Verde Oscuro Principal */
            --color-green-med: #225c3f;    /* Verde intermedio */
            --color-lime: #84cc16;         /* Verde Limón brillante */
            --color-lime-soft: #f1fbc6;    /* Verde Limón pálido */
            --color-blue-inst: #1e3a8a;    /* Azul Institucional (Colegio) */
            --color-blue-accent: #0288d1;  /* Azul / Celeste de contraste */
            --color-sky-blue: #e0f2fe;     /* Celeste suave de fondo */
            --color-dark-slate: #1e293b;   /* Texto principal de alto contraste */
            --color-gray-text: #475569;    /* Texto secundario */
            
            --font-serif: 'Playfair Display', serif;
            --font-sans: 'Plus Jakarta Sans', sans-serif;
            
            --transition-smooth: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
            --transition-fast: all 0.2s ease;
            --shadow-sm: 0 4px 12px rgba(20, 54, 37, 0.02);
            --shadow-md: 0 10px 30px rgba(20, 54, 37, 0.05);
            --shadow-lg: 0 20px 40px rgba(20, 54, 37, 0.08);
            --max-width: 1200px;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth;
            font-size: 16px;
        }

        body {
            font-family: var(--font-sans);
            color: var(--color-dark-slate);
            background-color: var(--color-white);
            line-height: 1.7;
            overflow-x: hidden;
        }

        h1, h2, h3, h4 {
            color: var(--color-dark-green);
            font-weight: 700;
        }

        /* Barra de progreso de lectura */
        .progress-bar {
            position: fixed;
            top: 0;
            left: 0;
            height: 4px;
            background: linear-gradient(to right, var(--color-lime), var(--color-blue-accent));
            width: 0%;
            z-index: 2000;
            transition: width 0.1s ease-out;
        }

        /* ==========================================================================
           2. COMPONENTES COMUNES (LAYOUT Y ESPACIADOS)
           ========================================================================== */
        .container {
            max-width: var(--max-width);
            margin: 0 auto;
            padding: 0 2rem;
        }

        .section {
            padding: 7rem 0;
            position: relative;
        }

        .bg-cream {
            background-color: var(--color-cream);
        }

        .bg-cream-light {
            background-color: var(--color-cream-light);
        }

        .grid {
            display: grid;
            gap: 3rem;
        }

        .grid-2 {
            grid-template-columns: repeat(2, 1fr);
        }

        .grid-3 {
            grid-template-columns: repeat(3, 1fr);
        }

        .align-center {
            align-items: center;
        }

        .text-center {
            text-align: center;
        }

        .mx-auto {
            margin-left: auto;
            margin-right: auto;
        }

        .mt-4 {
            margin-top: 3rem;
        }

        .max-w-xl {
            max-width: 700px;
        }

        .divider {
            height: 4px;
            width: 80px;
            background-color: var(--color-lime);
            margin-bottom: 2rem;
            border-radius: 20px;
        }

        .divider.center {
            margin-left: auto;
            margin-right: auto;
        }

        .section-tag {
            font-family: var(--font-sans);
            font-weight: 700;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-size: 0.85rem;
            color: var(--color-green-med);
            margin-bottom: 0.75rem;
            display: block;
        }

        .section-title {
            font-family: var(--font-serif);
            font-size: 2.75rem;
            line-height: 1.2;
            margin-bottom: 1.5rem;
        }

        .section-lead {
            font-size: 1.15rem;
            color: var(--color-gray-text);
            max-width: 700px;
            margin-bottom: 3rem;
        }

        /* Botones de alta fidelidad */
        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 0.75rem;
            padding: 1rem 2.25rem;
            border-radius: 50px;
            font-weight: 600;
            font-size: 0.95rem;
            cursor: pointer;
            transition: var(--transition-smooth);
            border: 2px solid transparent;
        }

        .btn-primary {
            background-color: var(--color-dark-green);
            color: var(--color-white);
            box-shadow: 0 10px 20px rgba(20, 54, 37, 0.15);
        }

        .btn-primary:hover {
            background-color: var(--color-green-med);
            transform: translateY(-3px);
            box-shadow: 0 15px 25px rgba(20, 54, 37, 0.25);
        }

        .btn-outline {
            background-color: transparent;
            color: var(--color-white);
            border-color: rgba(255, 255, 255, 0.4);
        }

        .btn-outline:hover {
            background-color: var(--color-white);
            color: var(--color-dark-green);
            transform: translateY(-3px);
            border-color: var(--color-white);
        }

        .btn-block {
            display: block;
            width: 100%;
        }

        /* Tarjetas de Identidad */
        .card {
            background-color: var(--color-white);
            border-radius: 16px;
            padding: 3rem 2rem;
            box-shadow: var(--shadow-sm);
            border: 1px solid rgba(20, 54, 37, 0.03);
            transition: var(--transition-smooth);
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-lg);
            border-color: rgba(132, 204, 22, 0.15);
        }

        .card-icon {
            font-size: 2.75rem;
            color: var(--color-green-med);
            margin-bottom: 1.5rem;
            display: inline-block;
        }

        .card h3 {
            font-family: var(--font-sans);
            font-size: 1.35rem;
            margin-bottom: 1rem;
        }

        /* ==========================================================================
           3. CABECERA Y NAVEGACIÓN FIXED
           ========================================================================== */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(15px);
            box-shadow: var(--shadow-sm);
            z-index: 1500;
            transition: var(--transition-smooth);
            border-bottom: 1px solid rgba(20, 54, 37, 0.05);
        }

        .nav-container {
            max-width: var(--max-width);
            margin: 0 auto;
            padding: 1.25rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: var(--transition-smooth);
        }

        .nav-logo {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            font-size: 1.35rem;
            font-weight: 800;
            color: var(--color-dark-green);
        }

        .logo-vector {
            width: 44px;
            height: 44px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--color-dark-green), var(--color-lime));
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--color-white);
            font-size: 1.15rem;
            font-weight: 800;
        }

        .nav-logo span {
            font-family: var(--font-serif);
        }

        .logo-accent {
            color: var(--color-blue-accent);
            font-family: var(--font-sans);
        }

        .nav-list {
            list-style: none;
            display: flex;
            gap: 1.75rem;
        }

        .nav-link {
            font-size: 0.9rem;
            font-weight: 600;
            color: var(--color-gray-text);
            padding: 0.5rem 0;
            position: relative;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 3px;
            background-color: var(--color-lime);
            border-radius: 10px;
            transition: var(--transition-smooth);
        }

        .nav-link:hover::after,
        .nav-link.active::after {
            width: 100%;
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--color-dark-green);
        }

        .nav-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--color-dark-green);
            cursor: pointer;
        }

        /* ==========================================================================
           4. PORTADA (HERO) - ESTILO EDITORIAL SIN IMAGEN
           ========================================================================== */
        .hero {
            position: relative;
            height: 100vh;
            min-height: 650px;
            /* Reemplazo de imagen de fondo por gradiente y patrón vectorial CSS */
            background-color: var(--color-dark-green);
            background-image: 
                radial-gradient(circle at 80% 20%, rgba(132, 204, 22, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 10% 80%, rgba(2, 136, 209, 0.1) 0%, transparent 50%);
            display: flex;
            align-items: center;
            color: var(--color-white);
            padding-top: 80px;
        }

        .hero-content {
            position: relative;
            z-index: 5;
            max-width: 850px;
        }

        .hero-tag {
            font-weight: 700;
            text-transform: uppercase;
            font-size: 0.85rem;
            letter-spacing: 4px;
            display: inline-block;
            margin-bottom: 1.5rem;
            background-color: rgba(255, 255, 255, 0.1);
            padding: 0.5rem 1.25rem;
            border-radius: 50px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.15);
        }

        .hero h1 {
            font-family: var(--font-serif);
            font-size: 4.5rem;
            color: var(--color-white);
            line-height: 1.1;
            margin-bottom: 1.5rem;
            text-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
        }

        .hero p {
            font-size: 1.6rem;
            margin-bottom: 3rem;
            font-weight: 300;
            font-family: var(--font-serif);
            font-style: italic;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.15);
        }

        .hero-actions {
            display: flex;
            gap: 1.25rem;
        }

        .hero-wave {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            overflow: hidden;
            line-height: 0;
            z-index: 6;
        }

        .hero-wave svg {
            position: relative;
            display: block;
            width: calc(100% + 1.3px);
            height: 60px;
        }

        /* ==========================================================================
           5. SECCIÓN GEOGRAFÍA / UBICACIÓN
           ========================================================================== */
        .location-info {
            background-color: var(--color-white);
            border-radius: 20px;
            padding: 3.5rem;
            box-shadow: var(--shadow-md);
            border-left: 6px solid var(--color-blue-accent);
        }

        .map-icon-box {
            font-size: 3rem;
            color: var(--color-blue-accent);
            margin-bottom: 1.5rem;
        }

        .geo-illustration {
            border: 1px solid rgba(20, 54, 37, 0.08);
            border-radius: 20px;
            background-color: var(--color-cream);
            padding: 3.5rem;
            text-align: center;
        }

        .geo-illustration i {
            font-size: 5rem;
            color: var(--color-green-med);
            margin-bottom: 1.5rem;
        }

        /* ==========================================================================
           6. SECCIÓN COLEGIO HORACIO ZEBALLOS (TEMA AZUL / CELESTE)
           ========================================================================== */
        .section-school {
            background-color: var(--color-blue-inst);
            color: var(--color-white);
        }

        .section-school .section-subtitle,
        .section-school h2,
        .section-school h3,
        .section-school h4,
        .section-school p {
            color: var(--color-white);
        }

        .section-school .divider {
            background: linear-gradient(to right, var(--color-blue-accent), var(--color-white));
        }

        .school-vector-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1.5rem;
        }

        .school-logo-box-vector {
            background-color: var(--color-white);
            padding: 2.5rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            grid-column: span 2;
            border-radius: 16px;
            color: var(--color-blue-inst);
            box-shadow: var(--shadow-sm);
        }

        .school-logo-box-vector i {
            font-size: 4.5rem;
            color: var(--color-blue-inst);
        }

        .school-logo-box-vector p {
            color: var(--color-blue-inst) !important;
            font-weight: 800;
            margin-top: 1rem;
            font-size: 1.25rem;
        }

        .school-vector-card {
            background-color: rgba(255, 255, 255, 0.08);
            border-radius: 12px;
            padding: 2rem;
            border: 1px solid rgba(255, 255, 255, 0.15);
            transition: var(--transition-smooth);
        }

        .school-vector-card:hover {
            background-color: rgba(255, 255, 255, 0.15);
            transform: translateY(-3px);
        }

        .school-vector-card i {
            font-size: 2rem;
            color: var(--color-sky-blue);
            margin-bottom: 1rem;
            display: block;
        }

        .school-list {
            list-style: none;
            margin-top: 1.5rem;
        }

        .school-list li {
            margin-bottom: 0.75rem;
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }

        .school-list li i {
            color: var(--color-lime);
        }

        /* ==========================================================================
           7. AGRICULTURA - REJILLA DE CULTIVOS
           ========================================================================== */
        .crop-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 1.25rem;
            margin-top: 2.5rem;
        }

        .crop-card {
            background-color: var(--color-white);
            border-radius: 16px;
            padding: 2rem 1.5rem;
            text-align: center;
            box-shadow: var(--shadow-sm);
            border: 1px solid rgba(20, 54, 37, 0.04);
            transition: var(--transition-smooth);
        }

        .crop-card:hover {
            transform: translateY(-5px);
            border-color: var(--color-lime);
            box-shadow: var(--shadow-md);
        }

        .crop-emoji {
            font-size: 2.75rem;
            margin-bottom: 1rem;
            display: block;
        }

        .crop-card span {
            font-weight: 700;
            font-size: 1rem;
            color: var(--color-dark-green);
        }

        .importance-list {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 1.25rem;
            margin-top: 2rem;
        }

        .importance-item {
            display: flex;
            gap: 1rem;
            align-items: flex-start;
        }

        .importance-icon {
            background-color: var(--color-lime-soft);
            color: var(--color-dark-green);
            font-size: 1rem;
            width: 32px;
            height: 32px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
            font-weight: 700;
        }

        /* ==========================================================================
           8. SOSTENIBILIDAD Y PASOS
           ========================================================================== */
        .sustain-steps {
            display: flex;
            flex-direction: column;
            gap: 2rem;
            margin-top: 2rem;
        }

        .sustain-step {
            display: flex;
            gap: 1.5rem;
            align-items: flex-start;
        }

        .sustain-number {
            background-color: var(--color-lime);
            color: var(--color-dark-green);
            font-weight: 800;
            font-size: 1.15rem;
            width: 44px;
            height: 44px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
            box-shadow: 0 4px 10px rgba(132, 204, 22, 0.2);
        }

        .sustain-step h4 {
            font-family: var(--font-sans);
            font-size: 1.15rem;
            margin-bottom: 0.35rem;
        }

        .sustain-step p {
            color: var(--color-gray-text);
        }

        /* ==========================================================================
           9. DATOS CURIOSOS (TARJETAS INTERACTIVAS)
           ========================================================================== */
        .fact-card {
            background-color: var(--color-cream);
            border-radius: 20px;
            padding: 3rem 2rem;
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(20, 54, 37, 0.05);
            transition: var(--transition-smo
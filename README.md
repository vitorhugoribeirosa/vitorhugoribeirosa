<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Vitor Hugo - Desenvolvedor</title>
    <style>
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        @keyframes slideIn {
            from { transform: translateX(-100%); }
            to { transform: translateX(0); }
        }

        @keyframes cardHover {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #141414;
            color: white;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }
        .navbar {
            display: flex;
            justify-content: space-between;
            padding: 20px;
            background-color: black;
            animation: fadeIn 1s ease-out;
        }
        .logo {
            color: red;
            font-size: 24px;
            font-weight: bold;
            animation: pulse 2s infinite;
        }
        .menu {
            display: flex;
            gap: 20px;
            animation: slideIn 1s ease-out;
        }
        .menu a {
            color: white;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        .menu a:hover {
            color: #e50914;
        }
        .hero {
            background-image: url('/api/placeholder/1200/600');
            height: 70vh;
            background-size: cover;
            display: flex;
            align-items: center;
            padding: 0 50px;
            animation: fadeIn 1.5s ease-out;
        }
        .hero-content {
            max-width: 500px;
            background-color: rgba(0,0,0,0.7);
            padding: 20px;
            border-radius: 10px;
            animation: slideIn 1.5s ease-out;
        }
        .row {
            display: flex;
            overflow-x: scroll;
            padding: 20px;
            gap: 10px;
            scroll-behavior: smooth;
        }
        .project-card {
            min-width: 200px;
            height: 300px;
            background-color: #333;
            border-radius: 5px;
            padding: 15px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            transition: all 0.3s ease;
            animation: fadeIn 2s ease-out;
        }
        .project-card:hover {
            transform: scale(1.05);
            box-shadow: 0 0 20px rgba(229, 9, 20, 0.5);
            animation: cardHover 0.5s ease;
        }
        .project-card h3 {
            color: #e50914;
            margin: 0;
            transition: color 0.3s ease;
        }
        .project-card:hover h3 {
            color: white;
        }
        .project-techs {
            display: flex;
            gap: 10px;
        }
        .tech-badge {
            background-color: #e50914;
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 12px;
            transition: transform 0.3s ease;
        }
        .tech-badge:hover {
            transform: scale(1.1);
        }
        /* Scrollbar Styling */
        .row::-webkit-scrollbar {
            height: 8px;
        }
        .row::-webkit-scrollbar-track {
            background: #333;
        }
        .row::-webkit-scrollbar-thumb {
            background: #e50914;
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <nav class="navbar">
        <div class="logo">DevStream</div>
        <div class="menu">
            <a href="#">Projetos</a>
            <a href="#">Sobre</a>
            <a href="#">Contato</a>
            <a href="#">GitHub</a>
        </div>
    </nav>

    <header class="hero">
        <div class="hero-content">
            <h1>Vitor Hugo</h1>
            <p>Técnico em Informática | Estudante de Sistemas da Informação</p>
            <p>Desenvolvedor apaixonado por tecnologia e criação de soluções inovadoras</p>
        </div>
    </header>

    <section>
        <h2>Projetos Principais</h2>
        <div class="row">
            <div class="project-card">
                <div>
                    <h3>StreamFlix</h3>
                    <p>Clone de interface de streaming</p>
                </div>
                <div class="project-techs">
                    <span class="tech-badge">HTML</span>
                    <span class="tech-badge">CSS</span>
                </div>
            </div>
            <div class="project-card">
                <div>
                    <h3>Sistema de Gestão</h3>
                    <p>Aplicação para gerenciamento de recursos</p>
                </div>
                <div class="project-techs">
                    <span class="tech-badge">Python</span>
                    <span class="tech-badge">Django</span>
                </div>
            </div>
            <div class="project-card">
                <div>
                    <h3>Portfólio Pessoal</h3>
                    <p>Site para apresentação de projetos</p>
                </div>
                <div class="project-techs">
                    <span class="tech-badge">React</span>
                    <span class="tech-badge">JavaScript</span>
                </div>
            </div>
        </div>
    </section>
</body>
</html>


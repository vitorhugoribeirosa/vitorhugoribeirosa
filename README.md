<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <title>Vitor Hugo - Desenvolvedor</title>
    <style>
        /* Animações nativas CSS */
        @keyframes slide-in {
            from { transform: translateX(-100%); opacity: 0; }
            to { transform: translateX(0); opacity: 1; }
        }

        @keyframes fade-in {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.1); }
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            background-color: #141414;
            color: white;
            line-height: 1.6;
        }

        /* Navbar com animação */
        .navbar {
            display: flex;
            justify-content: space-between;
            padding: 20px;
            background-color: black;
            animation: slide-in 1s ease;
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
        }

        .menu a {
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }

        .menu a:hover {
            color: red;
        }

        /* Seção principal */
        .profile {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            animation: fade-in 2s;
        }

        .hero {
            background-color: rgba(0,0,0,0.7);
            padding: 40px;
            text-align: center;
            border-radius: 10px;
            margin-bottom: 30px;
        }

        .hero h1 {
            color: red;
            margin-bottom: 10px;
        }

        /* Carrossel de projetos */
        .projects {
            display: flex;
            overflow-x: auto;
            gap: 20px;
            padding: 20px;
            scroll-snap-type: x mandatory;
        }

        .project-card {
            flex: 0 0 250px;
            background-color: #333;
            border-radius: 10px;
            padding: 20px;
            scroll-snap-align: center;
            transition: transform 0.3s;
        }

        .project-card:hover {
            transform: scale(1.05);
        }

        .project-card h3 {
            color: red;
            margin-bottom: 10px;
        }

        .tech-badges {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }

        .badge {
            background-color: red;
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8em;
        }

        /* Scrollbar personalizada */
        .projects::-webkit-scrollbar {
            height: 8px;
        }

        .projects::-webkit-scrollbar-track {
            background: #222;
        }

        .projects::-webkit-scrollbar-thumb {
            background-color: red;
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
        </div>
    </nav>

    <div class="profile">
        <div class="hero">
            <h1>Vitor Hugo</h1>
            <p>Técnico em Informática | Sistemas da Informação</p>
            <p>Desenvolvedor apaixonado por tecnologia</p>
        </div>

        <div class="projects">
            <div class="project-card">
                <h3>StreamFlix</h3>
                <p>Clone de interface de streaming</p>
                <div class="tech-badges">
                    <span class="badge">HTML</span>
                    <span class="badge">CSS</span>
                </div>
            </div>

            <div class="project-card">
                <h3>Sistema Gestão</h3>
                <p>Aplicação de gerenciamento</p>
                <div class="tech-badges">
                    <span class="badge">Python</span>
                    <span class="badge">Django</span>
                </div>
            </div>

            <div class="project-card">
                <h3>Portfólio</h3>
                <p>Site de apresentação pessoal</p>
                <div class="tech-badges">
                    <span class="badge">React</span>
                    <span class="badge">JS</span>
                </div>
            </div>
        </div>
    </div>
</body>
</html>

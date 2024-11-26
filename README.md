<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=OrestesFerraz&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dracula&locale=en&hide_border=false&order=1" height="150" alt="stats graph"  />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=OrestesFerraz&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false&order=2" height="150" alt="languages graph"  />
</div>

###

<div align="center">
  <img src="https://profile-counter.glitch.me/OrestesFerraz/count.svg?"  />
</div>

###

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Site Dark com Animação</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
</head>
<body>
    <!-- Cabeçalho, Navbar e Rodapé -->
    <div id="header-navbar-footer">
        <header>
            <h1>Meu Site</h1>
        </header>
        <nav id="navbar">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">Sobre</a></li>
                <li><a href="#contact">Contato</a></li>
            </ul>
        </nav>
        <button id="toggle-nav">☰</button>
        <footer>
            <p>&copy; 2024 Meu Site. Todos os direitos reservados.</p>
        </footer>
    </div>

    <!-- Conteúdo principal -->
    <main>
        <h1>Bem-vindo ao Meu Site!</h1>
        <p>Explore este exemplo de layout com tema dark e uma barra de navegação animada que desliza da direita.</p>
    </main>

    <script>
        // JavaScript para animação da navbar
        document.addEventListener("DOMContentLoaded", () => {
            const toggleNav = document.getElementById("toggle-nav");
            const navbar = document.getElementById("navbar");

            toggleNav.addEventListener("click", () => {
                navbar.classList.toggle("show");
            });
        });
    </script>

    <style>
        /* Estilo geral com tema dark */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #f0f0f0;
        }

        header {
            background-color: #1f1f1f;
            color: #f0f0f0;
            padding: 1rem;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        main {
            padding: 2rem;
            text-align: center;
        }

        footer {
            background-color: #1f1f1f;
            color: #f0f0f0;
            text-align: center;
            padding: 1rem;
            position: fixed;
            width: 100%;
            bottom: 0;
        }

        /* Estilo do navbar */
        #navbar {
            position: fixed;
            top: 0;
            right: -250px;
            height: 100%;
            width: 250px;
            background-color: #242424;
            box-shadow: -4px 0 6px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            padding: 1rem;
            transition: right 0.3s ease-in-out;
        }

        #navbar.show {
            right: 0;
        }

        #navbar ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        #navbar ul li {
            margin: 1rem 0;
        }

        #navbar ul li a {
            color: #f0f0f0;
            text-decoration: none;
            font-size: 1.2rem;
            transition: color 0.2s;
        }

        #navbar ul li a:hover {
            color: #1db954; /* Verde Spotify */
        }

        /* Botão do toggle */
        #toggle-nav {
            position: fixed;
            top: 1rem;
            right: 1rem;
            background-color: #1f1f1f;
            color: #f0f0f0;
            border: none;
            font-size: 1.5rem;
            padding: 0.5rem 1rem;
            cursor: pointer;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: background-color 0.2s;
        }

        #toggle-nav:hover {
            background-color: #1db954;
        }

        /* Mobile-first responsivo */
        @media (max-width: 600px) {
            main {
                padding: 1rem;
            }

            #navbar ul li a {
                font-size: 1rem;
            }
        }
    </style>
</body>
</html>
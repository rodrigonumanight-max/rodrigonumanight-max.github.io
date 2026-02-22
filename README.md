<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>RVO MUSIC - Portfólio de Pagode</title>
    <link rel="stylesheet" href="css/style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- HEADER/NAVEGAÇÃO -->
    <header class="navbar">
        <div class="container">
            <div class="logo">
                <h1>RVO MUSIC</h1>
            </div>
            <nav class="nav-menu">
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#sobre">Sobre</a></li>
                    <li><a href="#musicas">Músicas</a></li>
                    <li><a href="#contato">Contato</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- SEÇÃO HOME/CAPA -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>RVO MUSIC</h1>
            <p>Pagode de Qualidade</p>
            <p class="subtitle">33 Músicas de Pura Alegria e Tradição</p>
            <a href="#musicas" class="btn-primary">Ouça Agora</a>
        </div>
    </section>

    <!-- SEÇÃO SOBRE -->
    <section id="sobre" class="sobre">
        <div class="container">
            <h2>Sobre RVO MUSIC</h2>
            <div class="sobre-content">
                <div class="sobre-texto">
                    <p>Bem-vindo ao meu portfólio musical! Sou Rodrigo Numa Night, um apaixonado por pagode autêntico e de qualidade.</p>
                    <p>Tenho 33 músicas originais que refletem minha paixão pelo gênero, com letras que falam de alegria, amor e tradição.</p>
                    <p>Cada música é uma história, cada ritmo é um convite para dançar e curtir a vida ao som do verdadeiro pagode.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SEÇÃO MÚSICAS -->
    <section id="musicas" class="musicas">
        <div class="container">
            <h2>Minhas Músicas</h2>
            <div class="musicas-grid" id="musicasContainer">
                <!-- As músicas serão carregadas aqui via JavaScript -->
            </div>
        </div>
    </section>

    <!-- SEÇÃO CONTATO -->
    <section id="contato" class="contato">
        <div class="container">
            <h2>Contato & Redes Sociais</h2>
            <div class="social-links">
                <a href="https://instagram.com/rodrigo.numa.night" target="_blank" class="social-btn">
                    <i class="fab fa-instagram"></i> Instagram
                </a>
                <a href="mailto:contato@rvomusic.com" class="social-btn">
                    <i class="fas fa-envelope"></i> Email
                </a>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer class="footer">
        <p>&copy; 2026 RVO MUSIC. Todos os direitos reservados.</p>
    </footer>

    <script src="js/script.js"></script>
</body>
</html>* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #0a0a0a;
    color: #fff;
    line-height: 1.6;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* NAVBAR */
.navbar {
    background-color: #1a1a1a;
    padding: 20px 0;
    position: sticky;
    top: 0;
    z-index: 100;
    border-bottom: 2px solid #d4af37;
}

.navbar .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo h1 {
    font-size: 28px;
    color: #d4af37;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.8);
}

.nav-menu ul {
    display: flex;
    list-style: none;
    gap: 30px;
}

.nav-menu a {
    color: #fff;
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
}

.nav-menu a:hover {
    color: #d4af37;
}

/* HERO SECTION */
.hero {
    background: linear-gradient(135deg, #1a1a1a 0%, #2a2a2a 100%);
    padding: 120px 20px;
    text-align: center;
    border-bottom: 2px solid #d4af37;
}

.hero-content h1 {
    font-size: 64px;
    margin-bottom: 10px;
    color: #d4af37;
    text-shadow: 3px 3px 6px rgba(0,0,0,0.9);
}

.hero-content p {
    font-size: 24px;
    margin-bottom: 10px;
    color: #ccc;
}

.hero-content .subtitle {
    font-size: 18px;
    margin-bottom: 30px;
    color: #999;
}

.btn-primary {
    display: inline-block;
    background-color: #d4af37;
    color: #000;
    padding: 15px 40px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: 700;
    font-size: 16px;
    transition: all 0.3s ease;
    cursor: pointer;
}

.btn-primary:hover {
    background-color: #e8c547;
    transform: scale(1.05);
}

/* SOBRE SECTION */
.sobre {
    padding: 80px 20px;
    background-color: #0a0a0a;
}

.sobre h2 {
    font-size: 48px;
    margin-bottom: 40px;
    text-align: center;
    color: #d4af37;
}

.sobre-content {
    max-width: 800px;
    margin: 0 auto;
}

.sobre-texto p {
    font-size: 18px;
    margin-bottom: 20px;
    color: #ccc;
    line-height: 1.8;
}

/* MUSICAS SECTION */
.musicas {
    padding: 80px 20px;
    background-color: #1a1a1a;
}

.musicas h2 {
    font-size: 48px;
    margin-bottom: 50px;
    text-align: center;
    color: #d4af37;
}

.musicas-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
}

.musica-card {
    background-color: #2a2a2a;
    border: 2px solid #d4af37;
    border-radius: 10px;
    padding: 20px;
    transition: all 0.3s ease;
    cursor: pointer;
}

.musica-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 30px rgba(212, 175, 55, 0.3);
}

.musica-card h3 {
    color: #d4af37;
    margin-bottom: 10px;
    font-size: 18px;
}

.musica-card p {
    color: #999;
    font-size: 14px;
    margin-bottom: 15px;
}

.musica-card audio {
    width: 100%;
    margin-top: 15px;
}

/* CONTATO SECTION */
.contato {
    padding: 80px 20px;
    background-color: #0a0a0a;
    text-align: center;
}

.contato h2 {
    font-size: 48px;
    margin-bottom: 50px;
    color: #d4af37;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.social-btn {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    background-color: #d4af37;
    color: #000;
    padding: 15px 30px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: 700;
    transition: all 0.3s ease;
}

.social-btn:hover {
    background-color: #e8c547;
    transform: scale(1.05);
}

/* FOOTER */
.footer {
    background-color: #1a1a1a;
    padding: 20px;
    text-align: center;
    border-top: 2px solid #d4af37;
    color: #999;
}

/* RESPONSIVE */
@media (max-width: 768px) {
    .hero-content h1 {
        font-size: 40px;
    }

    .hero-content p {
        font-size: 18px;
    }

    .nav-menu ul {
        gap: 15px;
        font-size: 14px;
    }

    .musicas-grid {
        grid-template-columns: 1fr;
    }

    .social-links {
        flex-direction: column;
        align-items: center;
    }

    .social-btn {
        width: 100%;
        max-width: 300px;
    }
}// Array com as 33 músicas (você pode adicionar as URLs reais depois)
const musicas = [
    { id: 1, titulo: "Música 1", artista: "RVO MUSIC", arquivo: "musicas/musica-1.mp3" },
    { id: 2, titulo: "Música 2", artista: "RVO MUSIC", arquivo: "musicas/musica-2.mp3" },
    { id: 3, titulo: "Música 3", artista: "RVO MUSIC", arquivo: "musicas/musica-3.mp3" },
    { id: 4, titulo: "Música 4", artista: "RVO MUSIC", arquivo: "musicas/musica-4.mp3" },
    { id: 5, titulo: "Música 5", artista: "RVO MUSIC", arquivo: "musicas/musica-5.mp3" },
    { id: 6, titulo: "Música 6", artista: "RVO MUSIC", arquivo: "musicas/musica-6.mp3" },
    { id: 7, titulo: "Música 7", artista: "RVO MUSIC", arquivo: "musicas/musica-7.mp3" },
    { id: 8, titulo: "Música 8", artista: "RVO MUSIC", arquivo: "musicas/musica-8.mp3" },
    { id: 9, titulo: "Música 9", artista: "RVO MUSIC", arquivo: "musicas/musica-9.mp3" },
    { id: 10, titulo: "Música 10", artista: "RVO MUSIC", arquivo: "musicas/musica-10.mp3" },
    { id: 11, titulo: "Música 11", artista: "RVO MUSIC", arquivo: "musicas/musica-11.mp3" },
    { id: 12, titulo: "Música 12", artista: "RVO MUSIC", arquivo: "musicas/musica-12.mp3" },
    { id: 13, titulo: "Música 13", artista: "RVO MUSIC", arquivo: "musicas/musica-13.mp3" },
    { id: 14, titulo: "Música 14", artista: "RVO MUSIC", arquivo: "musicas/musica-14.mp3" },
    { id: 15, titulo: "Música 15", artista: "RVO MUSIC", arquivo: "musicas/musica-15.mp3" },
    { id: 16, titulo: "Música 16", artista: "RVO MUSIC", arquivo: "musicas/musica-16.mp3" },
    { id: 17, titulo: "Música 17", artista: "RVO MUSIC", arquivo: "musicas/musica-17.mp3" },
    { id: 18, titulo: "Música 18", artista: "RVO MUSIC", arquivo: "musicas/musica-18.mp3" },
    { id: 19, titulo: "Música 19", artista: "RVO MUSIC", arquivo: "musicas/musica-19.mp3" },
    { id: 20, titulo: "Música 20", artista: "RVO MUSIC", arquivo: "musicas/musica-20.mp3" },
    { id: 21, titulo: "Música 21", artista: "RVO MUSIC", arquivo: "musicas/musica-21.mp3" },
    { id: 22, titulo: "Música 22", artista: "RVO MUSIC", arquivo: "musicas/musica-22.mp3" },
    { id: 23, titulo: "Música 23", artista: "RVO MUSIC", arquivo: "musicas/musica-23.mp3" },
    { id: 24, titulo: "Música 24", artista: "RVO MUSIC", arquivo: "musicas/musica-24.mp3" },
    { id: 25, titulo: "Música 25", artista: "RVO MUSIC", arquivo: "musicas/musica-25.mp3" },
    { id: 26, titulo: "Música 26", artista: "RVO MUSIC", arquivo: "musicas/musica-26.mp3" },
    { id: 27, titulo: "Música 27", artista: "RVO MUSIC", arquivo: "musicas/musica-27.mp3" },
    { id: 28, titulo: "Música 28", artista: "RVO MUSIC", arquivo: "musicas/musica-28.mp3" },
    { id: 29, titulo: "Música 29", artista: "RVO MUSIC", arquivo: "musicas/musica-29.mp3" },
    { id: 30, titulo: "Música 30", artista: "RVO MUSIC", arquivo: "musicas/musica-30.mp3" },
    { id: 31, titulo: "Música 31", artista: "RVO MUSIC", arquivo: "musicas/musica-31.mp3" },
    { id: 32, titulo: "Música 32", artista: "RVO MUSIC", arquivo: "musicas/musica-32.mp3" },
    { id: 33, titulo: "Música 33", artista: "RVO MUSIC", arquivo: "musicas/musica-33.mp3" }
];

// Função para carregar e exibir as músicas
function carregarMusicas() {
    const container = document.getElementById('musicasContainer');
    
    musicas.forEach(musica => {
        const musicaCard = document.createElement('div');
        musicaCard.className = 'musica-card';
        musicaCard.innerHTML = `
            <h3>${musica.titulo}</h3>
            <p>${musica.artista}</p>
            <audio controls>
                <source src="${musica.arquivo}" type="audio/mpeg">
                Seu navegador não suporta o elemento de áudio.
            </audio>
        `;
        container.appendChild(musicaCard);
    });
}

// Executar quando a página carregar
document.addEventListener('DOMContentLoaded', carregarMusicas);

// Smooth scroll para os links de navegação
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({
                behavior: 'smooth'
            });
        }
    });
});// Array com as 33 músicas (você pode adicionar as URLs reais depois)
const musicas = [
    { id: 1, titulo: "Música 1", artista: "RVO MUSIC", arquivo: "musicas/musica-1.mp3" },
    { id: 2, titulo: "Música 2", artista: "RVO MUSIC", arquivo: "musicas/musica-2.mp3" },
    { id: 3, titulo: "Música 3", artista: "RVO MUSIC", arquivo: "musicas/musica-3.mp3" },
    { id: 4, titulo: "Música 4", artista: "RVO MUSIC", arquivo: "musicas/musica-4.mp3" },
    { id: 5, titulo: "Música 5", artista: "RVO MUSIC", arquivo: "musicas/musica-5.mp3" },
    { id: 6, titulo: "Música 6", artista: "RVO MUSIC", arquivo: "musicas/musica-6.mp3" },
    { id: 7, titulo: "Música 7", artista: "RVO MUSIC", arquivo: "musicas/musica-7.mp3" },
    { id: 8, titulo: "Música 8", artista: "RVO MUSIC", arquivo: "musicas/musica-8.mp3" },
    { id: 9, titulo: "Música 9", artista: "RVO MUSIC", arquivo: "musicas/musica-9.mp3" },
    { id: 10, titulo: "Música 10", artista: "RVO MUSIC", arquivo: "musicas/musica-10.mp3" },
    { id: 11, titulo: "Música 11", artista: "RVO MUSIC", arquivo: "musicas/musica-11.mp3" },
    { id: 12, titulo: "Música 12", artista: "RVO MUSIC", arquivo: "musicas/musica-12.mp3" },
    { id: 13, titulo: "Música 13", artista: "RVO MUSIC", arquivo: "musicas/musica-13.mp3" },
    { id: 14, titulo: "Música 14", artista: "RVO MUSIC", arquivo: "musicas/musica-14.mp3" },
    { id: 15, titulo: "Música 15", artista: "RVO MUSIC", arquivo: "musicas/musica-15.mp3" },
    { id: 16, titulo: "Música 16", artista: "RVO MUSIC", arquivo: "musicas/musica-16.mp3" },
    { id: 17, titulo: "Música 17", artista: "RVO MUSIC", arquivo: "musicas/musica-17.mp3" },
    { id: 18, titulo: "Música 18", artista: "RVO MUSIC", arquivo: "musicas/musica-18.mp3" },
    { id: 19, titulo: "Música 19", artista: "RVO MUSIC", arquivo: "musicas/musica-19.mp3" },
    { id: 20, titulo: "Música 20", artista: "RVO MUSIC", arquivo: "musicas/musica-20.mp3" },
    { id: 21, titulo: "Música 21", artista: "RVO MUSIC", arquivo: "musicas/musica-21.mp3" },
    { id: 22, titulo: "Música 22", artista: "RVO MUSIC", arquivo: "musicas/musica-22.mp3" },
    { id: 23, titulo: "Música 23", artista: "RVO MUSIC", arquivo: "musicas/musica-23.mp3" },
    { id: 24, titulo: "Música 24", artista: "RVO MUSIC", arquivo: "musicas/musica-24.mp3" },
    { id: 25, titulo: "Música 25", artista: "RVO MUSIC", arquivo: "musicas/musica-25.mp3" },
    { id: 26, titulo: "Música 26", artista: "RVO MUSIC", arquivo: "musicas/musica-26.mp3" },
    { id: 27, titulo: "Música 27", artista: "RVO MUSIC", arquivo: "musicas/musica-27.mp3" },
    { id: 28, titulo: "Música 28", artista: "RVO MUSIC", arquivo: "musicas/musica-28.mp3" },
    { id: 29, titulo: "Música 29", artista: "RVO MUSIC", arquivo: "musicas/musica-29.mp3" },
    { id: 30, titulo: "Música 30", artista: "RVO MUSIC", arquivo: "musicas/musica-30.mp3" },
    { id: 31, titulo: "Música 31", artista: "RVO MUSIC", arquivo: "musicas/musica-31.mp3" },
    { id: 32, titulo: "Música 32", artista: "RVO MUSIC", arquivo: "musicas/musica-32.mp3" },
    { id: 33, titulo: "Música 33", artista: "RVO MUSIC", arquivo: "musicas/musica-33.mp3" }
];

// Função para carregar e exibir as músicas
function carregarMusicas() {
    const container = document.getElementById('musicasContainer');
    
    musicas.forEach(musica => {
        const musicaCard = document.createElement('div');
        musicaCard.className = 'musica-card';
        musicaCard.innerHTML = `
            <h3>${musica.titulo}</h3>
            <p>${musica.artista}</p>
            <audio controls>
                <source src="${musica.arquivo}" type="audio/mpeg">
                Seu navegador não suporta o elemento de áudio.
            </audio>
        `;
        container.appendChild(musicaCard);
    });
}

// Executar quando a página carregar
document.addEventListener('DOMContentLoaded', carregarMusicas);

// Smooth scroll para os links de navegação
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({
                behavior: 'smooth'
            });
        }
    });
});// Array com as 33 músicas (você pode adicionar as URLs reais depois)
const musicas = [
    { id: 1, titulo: "Música 1", artista: "RVO MUSIC", arquivo: "musicas/musica-1.mp3" },
    { id: 2, titulo: "Música 2", artista: "RVO MUSIC", arquivo: "musicas/musica-2.mp3" },
    { id: 3, titulo: "Música 3", artista: "RVO MUSIC", arquivo: "musicas/musica-3.mp3" },
    { id: 4, titulo: "Música 4", artista: "RVO MUSIC", arquivo: "musicas/musica-4.mp3" },
    { id: 5, titulo: "Música 5", artista: "RVO MUSIC", arquivo: "musicas/musica-5.mp3" },
    { id: 6, titulo: "Música 6", artista: "RVO MUSIC", arquivo: "musicas/musica-6.mp3" },
    { id: 7, titulo: "Música 7", artista: "RVO MUSIC", arquivo: "musicas/musica-7.mp3" },
    { id: 8, titulo: "Música 8", artista: "RVO MUSIC", arquivo: "musicas/musica-8.mp3" },
    { id: 9, titulo: "Música 9", artista: "RVO MUSIC", arquivo: "musicas/musica-9.mp3" },
    { id: 10, titulo: "Música 10", artista: "RVO MUSIC", arquivo: "musicas/musica-10.mp3" },
    { id: 11, titulo: "Música 11", artista: "RVO MUSIC", arquivo: "musicas/musica-11.mp3" },
    { id: 12, titulo: "Música 12", artista: "RVO MUSIC", arquivo: "musicas/musica-12.mp3" },
    { id: 13, titulo: "Música 13", artista: "RVO MUSIC", arquivo: "musicas/musica-13.mp3" },
    { id: 14, titulo: "Música 14", artista: "RVO MUSIC", arquivo: "musicas/musica-14.mp3" },
    { id: 15, titulo: "Música 15", artista: "RVO MUSIC", arquivo: "musicas/musica-15.mp3" },
    { id: 16, titulo: "Música 16", artista: "RVO MUSIC", arquivo: "musicas/musica-16.mp3" },
    { id: 17, titulo: "Música 17", artista: "RVO MUSIC", arquivo: "musicas/musica-17.mp3" },
    { id: 18, titulo: "Música 18", artista: "RVO MUSIC", arquivo: "musicas/musica-18.mp3" },
    { id: 19, titulo: "Música 19", artista: "RVO MUSIC", arquivo: "musicas/musica-19.mp3" },
    { id: 20, titulo: "Música 20", artista: "RVO MUSIC", arquivo: "musicas/musica-20.mp3" },
    { id: 21, titulo: "Música 21", artista: "RVO MUSIC", arquivo: "musicas/musica-21.mp3" },
    { id: 22, titulo: "Música 22", artista: "RVO MUSIC", arquivo: "musicas/musica-22.mp3" },
    { id: 23, titulo: "Música 23", artista: "RVO MUSIC", arquivo: "musicas/musica-23.mp3" },
    { id: 24, titulo: "Música 24", artista: "RVO MUSIC", arquivo: "musicas/musica-24.mp3" },
    { id: 25, titulo: "Música 25", artista: "RVO MUSIC", arquivo: "musicas/musica-25.mp3" },
    { id: 26, titulo: "Música 26", artista: "RVO MUSIC", arquivo: "musicas/musica-26.mp3" },
    { id: 27, titulo: "Música 27", artista: "RVO MUSIC", arquivo: "musicas/musica-27.mp3" },
    { id: 28, titulo: "Música 28", artista: "RVO MUSIC", arquivo: "musicas/musica-28.mp3" },
    { id: 29, titulo: "Música 29", artista: "RVO MUSIC", arquivo: "musicas/musica-29.mp3" },
    { id: 30, titulo: "Música 30", artista: "RVO MUSIC", arquivo: "musicas/musica-30.mp3" },
    { id: 31, titulo: "Música 31", artista: "RVO MUSIC", arquivo: "musicas/musica-31.mp3" },
    { id: 32, titulo: "Música 32", artista: "RVO MUSIC", arquivo: "musicas/musica-32.mp3" },
    { id: 33, titulo: "Música 33", artista: "RVO MUSIC", arquivo: "musicas/musica-33.mp3" }
];

// Função para carregar e exibir as músicas
function carregarMusicas() {
    const container = document.getElementById('musicasContainer');
    
    musicas.forEach(musica => {
        const musicaCard = document.createElement('div');
        musicaCard.className = 'musica-card';
        musicaCard.innerHTML = `
            <h3>${musica.titulo}</h3>
            <p>${musica.artista}</p>
            <audio controls>
                <source src="${musica.arquivo}" type="audio/mpeg">
                Seu navegador não suporta o elemento de áudio.
            </audio>
        `;
        container.appendChild(musicaCard);
    });
}

// Executar quando a página carregar
document.addEventListener('DOMContentLoaded', carregarMusicas);

// Smooth scroll para os links de navegação
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({
                behavior: 'smooth'
            });
        }
    });
});# RVO MUSIC - Portfólio de Pagode

🎵 **Bem-vindo ao portfólio oficial de RVO MUSIC!**

Aqui você encontra as 33 músicas autorais de pagode de qualidade, criadas com paixão e tradição.

## 📊 Informações

- **Artista**: RVO MUSIC (Rodrigo Numa Night)
- **Total de Músicas**: 33
- **Gênero**: Pagode
- **Instagram**: [@rodrigo.numa.night](https://instagram.com/rodrigo.numa.night)

## 🌐 Acesse o site

O site está disponível em: `https://rodrigonumanight-max.github.io`

## 📁 Estrutura do Projeto

```
rodrigonumanight-max.github.io/
├── index.html          # Página principal
├── css/
│   └── style.css       # Estilos (tema preto e dourado)
├── js/
│   └── script.js       # Funcionalidades
├── musicas/            # Pasta para seus arquivos de áudio
│   ├── musica-1.mp3
│   ├── musica-2.mp3
│   └── ... (até musica-33.mp3)
├── imagens/            # Pasta para fotos e artes
└── README.md           # Este arquivo
```

## 🚀 Como adicionar suas músicas

1. Crie uma pasta `musicas` na raiz do repositório
2. Adicione seus arquivos MP3 nomeados como `musica-1.mp3`, `musica-2.mp3`, etc.
3. Atualize os nomes das músicas no array `musicas` em `js/script.js`

**Exemplo:**
```javascript
{ id: 1, titulo: "Nome da Sua Música", artista: "RVO MUSIC", arquivo: "musicas/musica-1.mp3" }
```

## 🎨 Personalização

### Cores
As cores principais podem ser alteradas em `css/style.css`:
- **Cor primária (dourado)**: `#d4af37`
- **Cor de fundo (preto)**: `#0a0a0a`

### Informações do Artista
Para alterar informações, edite a seção "SOBRE" no `index.html`

## 📱 Responsivo

O site é totalmente responsivo e funciona em:
- ✅ Desktop
- ✅ Tablets
- ✅ Dispositivos móveis

## 🔧 Tecnologias Utilizadas

- **HTML5** - Estrutura
- **CSS3** - Estilização (com gradientes e animações)
- **JavaScript** - Interatividade
- **GitHub Pages** - Hospedagem gratuita

## 💡 Dicas

- Substitua os nomes das músicas pelos títulos reais de suas faixas
- Adicione imagens em `imagens/` e referencie-as no HTML
- Use o GitHub Web Editor para editar diretamente pelo navegador

## 📞 Contato

- 📱 Instagram: [@rodrigo.numa.night](https://instagram.com/rodrigo.numa.night)
- 📧 Email: contato@rvomusic.com

---

**© 2026 RVO MUSIC. Todos os direitos reservados.**

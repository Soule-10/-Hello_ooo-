# -Hello_ooo-
Web
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- Métadonnées SEO -->
    <meta name="description" content="Institut Béninois de Formation et Partage du Savoir - Centre d'excellence pour les formations professionnelles au Bénin">
    <meta name="keywords" content="formation Bénin, éducation, apprentissage, certification, diplôme, cours, ateliers, séminaires, Cotonou">
    <meta name="author" content="Institut Béninois de Formation">
    
    <!-- Métadonnées Open Graph -->
    <meta property="og:title" content="IBFPS - Formation et Partage de Savoir au Bénin">
    <meta property="og:description" content="Découvrez nos programmes de formation adaptés aux besoins du marché béninois">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://www.ibfps-benin.org">
    <meta property="og:image" content="https://www.ibfps-benin.org/images/logo-social.jpg">
    <meta property="og:locale" content="fr_BJ">
    
    <!-- Favicon -->
    <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
    <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
    <link rel="manifest" href="/site.webmanifest">
    <link rel="mask-icon" href="/safari-pinned-tab.svg" color="#008751">
    <meta name="msapplication-TileColor" content="#008751">
    <meta name="theme-color" content="#ffffff">
    
    <!-- Préchargement -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link rel="preload" href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&family=Open+Sans:wght@400;600;700&display=swap" as="style" onload="this.onload=null;this.rel='stylesheet'">
    <noscript><link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&family=Open+Sans:wght@400;600;700&display=swap"></noscript>
    
    <!-- CSS -->
    <link rel="preload" href="style.css" as="style">
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    
    <!-- Scripts -->
    <script src="https://code.jquery.com/jquery-3.6.0.min.js" defer></script>
    <script src="script.js" defer></script>
    
    <title>IBFPS - Institut Béninois de Formation et Partage du Savoir</title>
    
    <!-- Style critique inline -->
    <style>
        :root {
            --primary: #fcd116;
            --secondary: #008751;
            --accent: #e8112d;
            --dark: #1a1a1a;
            --light: #f8f9fa;
            --text: #333333;
        }
        
        /* Style minimal pour le chargement initial */
        body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            color: var(--text);
            overflow-x: hidden;
        }
        
        header {
            background: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            transition: all 0.3s ease;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        /* Loader pour transition entre pages */
        #page-loader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: white;
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            transition: opacity 0.3s ease;
        }
        
        #page-loader .spinner {
            width: 50px;
            height: 50px;
            border: 5px solid var(--primary);
            border-radius: 50%;
            border-top-color: transparent;
            animation: spin 1s linear infinite;
        }
        
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        
        /* Accessibilité : skip to content */
        .skip-link {
            position: absolute;
            top: -40px;
            left: 0;
            background: var(--secondary);
            color: white;
            padding: 8px;
            z-index: 100;
            transition: top 0.3s;
        }
        
        .skip-link:focus {
            top: 0;
        }
    </style>
</head>
<body>
    <!-- Lien d'accessibilité -->
    <a href="#main-content" class="skip-link">Aller au contenu principal</a>
    
    <!-- Loader pour transition entre pages -->
    <div id="page-loader">
        <div class="spinner"></div>
    </div>
    
    <!-- Barre d'information supérieure -->
    <div class="top-bar bg-secondary text-white">
        <div class="container">
            <div class="d-flex justify-content-between">
                <div class="top-bar-info">
                    <span><i class="fas fa-phone-alt"></i> +229 XX XX XX XX</span>
                    <span><i class="fas fa-envelope"></i> contact@ibfps-benin.org</span>
                </div>
                <div class="top-bar-social">
                    <a href="#" aria-label="Facebook"><i class="fab fa-facebook-f"></i></a>
                    <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                    <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin-in"></i></a>
                    <a href="#" aria-label="WhatsApp"><i class="fab fa-whatsapp"></i></a>
                </div>
            </div>
        </div>
    </div>

    <!-- Navigation principale -->
    <header class="header">
        <div class="container">
            <nav class="navbar" aria-label="Navigation principale">
                <a href="index.html" class="logo">
                    <img src="images/logo.png" alt="Logo IBFPS" height="60">
                    <div class="logo-text">
                        <span class="text-secondary font-weight-bold">IBFPS</span>
                        <span class="text-accent small">Institut Béninois de Formation</span>
                    </div>
                </a>
                
                <button class="menu-toggle" id="mobile-menu" aria-label="Menu mobile" aria-expanded="false">
                    <span></span>
                    <span></span>
                    <span></span>
                </button>
                
                <ul class="nav-menu" id="main-nav">
                    <li><a href="index.html" class="active">Accueil</a></li>
                    <li><a href="about.html">À propos</a></li>
                    <li class="dropdown">
                        <a href="formations.html" aria-haspopup="true" aria-expanded="false">Formations <i class="fas fa-chevron-down"></i></a>
                        <ul class="dropdown-menu" aria-label="Sous-menu formations">
                            <li><a href="formations.html#professionnelles">Professionnelles</a></li>
                            <li><a href="formations.html#certifiantes">Certifiantes</a></li>
                            <li><a href="formations.html#ateliers">Ateliers</a></li>
                        </ul>
                    </li>
                    <li><a href="ressources.html">Ressources</a></li>
                    <li><a href="actualites.html">Actualités</a></li>
                    <li><a href="contact.html">Contact</a></li>
                    <li><a href="inscription.html" class="btn btn-primary">S'inscrire</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Contenu principal -->
    <main id="main-content">
        <!-- Le reste de votre contenu ici... -->
        
        <!-- Exemple de section -->
        <section class="hero">
            <div class="container">
                <h1>Bienvenue à l'IBFPS</h1>
                <p>Votre institut de formation professionnelle au Bénin</p>
            </div>
        </section>
    </main>

    <!-- Pied de page -->
    <footer>
        <!-- Votre pied de page ici... -->
    </footer>

    <!-- Script pour gérer les transitions -->
    <script>
        // Masquer le loader une fois la page chargée
        window.addEventListener('load', function() {
            document.getElementById('page-loader').style.opacity = '0';
            setTimeout(function() {
                document.getElementById('page-loader').style.display = 'none';
            }, 300);
            
            // Animation des liens pour une navigation fluide
            document.querySelectorAll('a[href^="#"], a[href^="http"]').forEach(link => {
                link.addEventListener('click', function(e) {
                    if(this.getAttribute('href').startsWith('http')) return;
                    
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if(target) {
                        target.scrollIntoView({
                            behavior: 'smooth'
                        });
                    }
                });
            });
        });
        
        // Menu mobile
        document.getElementById('mobile-menu').addEventListener('click', function() {
            this.setAttribute('aria-expanded', this.getAttribute('aria-expanded') === 'true' ? 'false' : 'true');
            document.getElementById('main-nav').classList.toggle('active');
        });
    </script>
</body>
</html>

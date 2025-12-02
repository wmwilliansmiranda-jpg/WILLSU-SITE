
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <!-- Google tag (gtag.js) -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=AW-17709030845"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'AW-17709030845');
    </script>
    
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="WILLSU - Restauração e Envelopamento Premium de Eletrodomésticos e Móveis. Deixe seus eletros como novos com técnica exclusiva.">
    <title>WILLSU - Restauração e Envelopamento Premium</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* RESET E CONFIGURAÇÕES GERAIS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #1a365d;
            --secondary: #2d74da;
            --accent: #e53e3e;
            --whatsapp: #25D366;
            --light: #f7fafc;
            --dark: #2d3748;
            --success: #38a169;
            --gray: #718096;
            --shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
            --shadow-hover: 0 20px 40px rgba(0, 0, 0, 0.15);
            --radius: 16px;
            --transition: all 0.3s ease;
        }

        body {
            font-family: 'Segoe UI', 'Inter', system-ui, -apple-system, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        .container {
            width: 100%;
            max-width: 1280px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* ANIMAÇÕES */
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

        /* HEADER */
        header {
            background: rgba(26, 54, 93, 0.95);
            color: white;
            padding: 1rem 0;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            backdrop-filter: blur(10px);
            animation: slideIn 0.5s ease-out;
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: relative;
        }

        .logo {
            font-size: 2rem;
            font-weight: 800;
            color: white;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo span {
            color: var(--secondary);
            position: relative;
        }

        .logo span::after {
            content: '';
            position: absolute;
            bottom: -2px;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
            border-radius: 2px;
        }

        .mobile-menu {
            font-size: 1.8rem;
            cursor: pointer;
            color: white;
            display: none;
            padding: 10px;
            border-radius: 8px;
            transition: var(--transition);
        }

        .mobile-menu:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            align-items: center;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            font-size: 1.1rem;
            padding: 8px 16px;
            border-radius: 8px;
            transition: var(--transition);
            position: relative;
        }

        .nav-links a:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateY(-2px);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            width: 0;
            height: 2px;
            background: var(--secondary);
            transition: all 0.3s ease;
            transform: translateX(-50%);
        }

        .nav-links a:hover::after {
            width: 80%;
        }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, #2c5282 100%);
            color: white;
            padding: 180px 0 100px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg width="60" height="60" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill="rgba(255,255,255,0.02)" d="M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z"/></g></svg>');
            animation: moveBackground 20s linear infinite;
        }

        @keyframes moveBackground {
            0% { transform: translate(0, 0); }
            100% { transform: translate(60px, 60px); }
        }

        .hero-content {
            max-width: 900px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
            animation: fadeIn 1s ease-out;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            line-height: 1.2;
            font-weight: 800;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
            color: white; /* ALTERAÇÃO SOLICITADA - Letras brancas */
        }

        .hero-subtitle {
            font-size: 1.5rem;
            margin-bottom: 2.5rem;
            opacity: 0.9;
            font-weight: 300;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn-whatsapp-hero {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            background: linear-gradient(135deg, var(--whatsapp) 0%, #1da851 100%);
            color: white;
            padding: 20px 45px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.3rem;
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(37, 211, 102, 0.3);
            border: none;
            cursor: pointer;
            animation: pulse 2s infinite;
        }

        .btn-whatsapp-hero:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 40px rgba(37, 211, 102, 0.4);
        }

        /* SECTIONS */
        section {
            padding: 100px 0;
            animation: fadeIn 0.8s ease-out;
        }

        .section-title {
            text-align: center;
            margin-bottom: 4rem;
            position: relative;
        }

        .section-title h2 {
            font-size: 2.8rem;
            color: var(--primary);
            margin-bottom: 1rem;
            font-weight: 800;
            position: relative;
            display: inline-block;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
            border-radius: 2px;
        }

        .section-title p {
            color: var(--gray);
            font-size: 1.2rem;
            max-width: 600px;
            margin: 1rem auto 0;
        }

        /* SERVICES */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .service-card {
            background: white;
            border-radius: var(--radius);
            padding: 2.5rem;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border: 1px solid rgba(0, 0, 0, 0.05);
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 100%;
            background: linear-gradient(to bottom, var(--secondary), var(--accent));
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-hover);
        }

        .service-icon {
            background: linear-gradient(135deg, var(--secondary), var(--accent));
            color: white;
            width: 70px;
            height: 70px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
            box-shadow: 0 10px 20px rgba(45, 116, 218, 0.2);
        }

        .service-content h3 {
            color: var(--primary);
            margin-bottom: 1.2rem;
            font-size: 1.6rem;
            font-weight: 700;
        }

        .service-content ul {
            list-style: none;
        }

        .service-content li {
            margin-bottom: 0.8rem;
            padding-left: 1.8rem;
            position: relative;
            color: var(--dark);
        }

        .service-content li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--success);
            font-weight: bold;
            font-size: 1.2rem;
        }

        /* PRICING */
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .price-card {
            background: white;
            border-radius: var(--radius);
            padding: 2.5rem 2rem;
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border: 2px solid transparent;
            position: relative;
            overflow: hidden;
        }

        .price-card::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
        }

        .price-card:hover {
            transform: translateY(-10px);
            border-color: var(--secondary);
            box-shadow: var(--shadow-hover);
        }

        .price-card h3 {
            color: var(--primary);
            margin-bottom: 1.5rem;
            font-size: 1.5rem;
            font-weight: 700;
        }

        .price-from {
            font-size: 1rem;
            color: var(--gray);
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .price {
            font-size: 2.8rem;
            font-weight: 800;
            color: var(--accent);
            margin: 1rem 0;
            position: relative;
        }

        .price::before {
            content: 'R$';
            font-size: 1.4rem;
            position: absolute;
            left: -1.5rem;
            top: 0.5rem;
        }

        /* TESTIMONIALS */
        .testimonials-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .testimonial-card {
            background: white;
            border-radius: var(--radius);
            padding: 2rem;
            box-shadow: var(--shadow);
            position: relative;
            transition: var(--transition);
        }

        .testimonial-card:hover {
            transform: translateY(-5px);
            box-shadow: var(--shadow-hover);
        }

        .testimonial-card::before {
            content: '"';
            font-size: 5rem;
            color: var(--secondary);
            position: absolute;
            top: -20px;
            left: 20px;
            opacity: 0.2;
            font-family: serif;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 1.5rem;
            padding-left: 1rem;
            color: var(--dark);
            line-height: 1.8;
            font-size: 1.1rem;
        }

        .testimonial-author {
            font-weight: 700;
            color: var(--primary);
            text-align: right;
            font-size: 1.1rem;
        }

        .testimonial-rating {
            color: #ffc107;
            margin-bottom: 1rem;
        }

        /* COVERAGE */
        .coverage-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
            gap: 1.2rem;
        }

        .city-card {
            background: white;
            border-radius: 10px;
            padding: 1.2rem;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: var(--transition);
            border: 1px solid #e2e8f0;
            font-weight: 500;
        }

        .city-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.1);
            border-color: var(--secondary);
        }

        /* ABOUT */
        .about-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 3rem;
        }

        .about-text h3 {
            color: var(--primary);
            margin-bottom: 1.5rem;
            font-size: 2rem;
            font-weight: 700;
        }

        .about-text p {
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
            line-height: 1.8;
            color: var(--dark);
        }

        /* CTA */
        .cta {
            background: linear-gradient(135deg, var(--primary) 0%, #2c5282 100%);
            color: white;
            text-align: center;
            padding: 100px 20px;
            position: relative;
            overflow: hidden;
        }

        .cta::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg width="60" height="60" xmlns="http://www.w3.org/2000/svg"><g fill="none" fill-rule="evenodd"><path fill="rgba(255,255,255,0.05)" d="M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z"/></g></svg>');
        }

        .cta-content {
            position: relative;
            z-index: 1;
            max-width: 800px;
            margin: 0 auto;
        }

        .cta h2 {
            font-size: 3rem;
            margin-bottom: 1.5rem;
            font-weight: 800;
        }

        .cta p {
            font-size: 1.3rem;
            margin-bottom: 3rem;
            opacity: 0.9;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .btn-whatsapp-cta {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: linear-gradient(135deg, var(--whatsapp) 0%, #1da851 100%);
            color: white;
            padding: 20px 45px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1.3rem;
            transition: var(--transition);
            box-shadow: 0 10px 30px rgba(37, 211, 102, 0.3);
            animation: pulse 2s infinite;
        }

        .btn-whatsapp-cta:hover {
            transform: translateY(-5px) scale(1.05);
            box-shadow: 0 15px 40px rgba(37, 211, 102, 0.4);
        }

        /* FOOTER */
        footer {
            background: var(--dark);
            color: white;
            padding: 80px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-bottom: 3rem;
        }

        .footer-column h3 {
            color: var(--secondary);
            margin-bottom: 1.5rem;
            font-size: 1.5rem;
            font-weight: 700;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background: var(--secondary);
            border-radius: 2px;
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column li {
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .footer-column a {
            color: #cbd5e0;
            text-decoration: none;
            transition: var(--transition);
            font-size: 1.1rem;
        }

        .footer-column a:hover {
            color: var(--secondary);
            transform: translateX(5px);
        }

        .social-icons {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            font-size: 1.2rem;
            transition: var(--transition);
        }

        .social-icons a:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 1rem;
            color: #a0aec0;
        }

        .privacy-link {
            text-align: center;
            margin-top: 1rem;
        }

        .privacy-link a {
            color: #a0aec0;
            text-decoration: none;
            font-size: 1rem;
            transition: var(--transition);
        }

        .privacy-link a:hover {
            color: var(--secondary);
        }

        /* WHATSAPP FLOAT */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 70px;
            height: 70px;
            background: linear-gradient(135deg, var(--whatsapp) 0%, #1da851 100%);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            box-shadow: 0 10px 30px rgba(37, 211, 102, 0.4);
            z-index: 1000;
            text-decoration: none;
            animation: pulse 2s infinite;
            transition: var(--transition);
        }

        .whatsapp-float:hover {
            transform: scale(1.1) rotate(10deg);
            box-shadow: 0 15px 40px rgba(37, 211, 102, 0.5);
        }

        .whatsapp-badge {
            position: absolute;
            top: -5px;
            right: -5px;
            background: var(--accent);
            color: white;
            font-size: 0.8rem;
            padding: 5px 10px;
            border-radius: 20px;
            font-weight: bold;
            animation: pulse 1.5s infinite;
        }

        /* RESPONSIVE */
        @media (max-width: 1024px) {
            .hero h1 {
                font-size: 3rem;
            }
            
            .section-title h2 {
                font-size: 2.5rem;
            }
        }

        @media (max-width: 768px) {
            .mobile-menu {
                display: block;
            }

            .nav-links {
                position: fixed;
                top: 70px;
                left: 0;
                right: 0;
                background: var(--primary);
                flex-direction: column;
                padding: 2rem;
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
                transform: translateY(-100%);
                opacity: 0;
                visibility: hidden;
                transition: all 0.3s ease;
                border-radius: 0 0 20px 20px;
                z-index: 999;
            }

            .nav-links.active {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }

            .hero {
                padding: 140px 0 80px;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero-subtitle {
                font-size: 1.3rem;
            }

            section {
                padding: 70px 0;
            }

            .section-title h2 {
                font-size: 2.2rem;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .btn-whatsapp-hero,
            .btn-whatsapp-cta {
                padding: 18px 35px;
                font-size: 1.2rem;
            }

            .cta h2 {
                font-size: 2.5rem;
            }

            .whatsapp-float {
                width: 60px;
                height: 60px;
                font-size: 1.8rem;
                bottom: 20px;
                right: 20px;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }

            .hero-subtitle {
                font-size: 1.1rem;
            }

            .section-title h2 {
                font-size: 1.8rem;
            }

            .service-card,
            .price-card,
            .testimonial-card {
                padding: 1.5rem;
            }

            .coverage-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            .btn-whatsapp-hero,
            .btn-whatsapp-cta {
                width: 100%;
                max-width: 300px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <a href="#" class="logo">
                    <i class="fas fa-home"></i>
                    WILL<span>SU</span>
                </a>
                <div class="mobile-menu" id="mobileMenu">
                    <i class="fas fa-bars"></i>
                </div>
                <nav class="nav-links" id="navLinks">
                    <a href="#servicos"><i class="fas fa-tools"></i> Serviços</a>
                    <a href="#precos"><i class="fas fa-tags"></i> Preços</a>
                    <a href="#depoimentos"><i class="fas fa-comments"></i> Depoimentos</a>
                    <a href="#cobertura"><i class="fas fa-map-marker-alt"></i> Área de Atuação</a>
                    <a href="#sobre"><i class="fas fa-info-circle"></i> Sobre</a>
                    <a href="#contato"><i class="fas fa-phone-alt"></i> Contato</a>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>TRANSFORMAMOS SEUS ELETRODOMÉSTICOS E MÓVEIS COM ADESIVOS E ACABAMENTO PREMIUM</h1>
                <p class="hero-subtitle">Deixe seus eletros como novos com técnica exclusiva e durabilidade garantida</p>
                <a href="https://wa.me/5511983357198?text=Olá%20WILLSU!%20Gostaria%20de%20solicitar%20um%20orçamento%20para%20transformação%20de%20eletrodomésticos%20e%20móveis." 
                   class="btn-whatsapp-hero"
                   target="_blank"
                   aria-label="Solicitar orçamento via WhatsApp">
                    <i class="fab fa-whatsapp"></i> SOLICITAR ORÇAMENTO AGORA
                </a>
                <p style="margin-top: 2rem; font-size: 0.9rem; opacity: 0.8;">
                    Atendimento rápido • Orçamento gratuito • Garantia total
                </p>
            </div>
        </div>
    </section>

    <!-- Serviços -->
    <section id="servicos">
        <div class="container">
            <div class="section-title">
                <h2>Nossos Serviços</h2>
                <p>Soluções completas de restauração e envelopamento premium</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-paint-roller"></i></div>
                    <div class="service-content">
                        <h3>Envelopamento Premium</h3>
                        <p>Cores modernas e alta durabilidade para:</p>
                        <ul>
                            <li>Geladeiras e Freezers</li>
                            <li>Fogões e Cooktops</li>
                            <li>Micro-ondas</li>
                            <li>Máquinas de lavar</li>
                            <li>Móveis planejados</li>
                            <li>Armários de cozinha</li>
                        </ul>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-hammer"></i></div>
                    <div class="service-content">
                        <h3>Restauração Completa</h3>
                        <p>Técnica exclusiva para recuperação total:</p>
                        <ul>
                            <li>Remoção de ferrugem e oxidação</li>
                            <li>Restauração de superfícies danificadas</li>
                            <li>Correção de amarelado e manchas</li>
                            <li>Troca de componentes estéticos</li>
                            <li>Preparação profissional</li>
                            <li>Acabamento impecável</li>
                        </ul>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-leaf"></i></div>
                    <div class="service-content">
                        <h3>Solução Sustentável</h3>
                        <p>Economia inteligente e ecológica:</p>
                        <ul>
                            <li>Até 80% mais econômico</li>
                            <li>Design moderno e atualizado</li>
                            <li>Redução de descarte eletrônico</li>
                            <li>Conservação de recursos</li>
                            <li>Materiais de alta qualidade</li>
                            <li>Processo limpo e seguro</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Preços -->
    <section id="precos" style="background: linear-gradient(135deg, #f0f7ff 0%, #e6f0ff 100%);">
        <div class="container">
            <div class="section-title">
                <h2>Nossos Preços</h2>
                <p>Investimento acessível com qualidade premium</p>
            </div>
            <div class="pricing-grid">
                <div class="price-card">
                    <h3>Geladeiras</h3>
                    <div class="price-from">A PARTIR DE</div>
                    <div class="price">500</div>
                    <p>Transformação completa</p>
                    <p style="font-size: 0.9rem; color: var(--gray); margin-top: 10px;">Valor base - depende do modelo</p>
                </div>
                <div class="price-card">
                    <h3>Fogões</h3>
                    <div class="price-from">A PARTIR DE</div>
                    <div class="price">300</div>
                    <p>Renovação completa</p>
                    <p style="font-size: 0.9rem; color: var(--gray); margin-top: 10px;">Inclui tampo e forno</p>
                </div>
                <div class="price-card">
                    <h3>Micro-ondas</h3>
                    <div class="price-from">A PARTIR DE</div>
                    <div class="price">180</div>
                    <p>Envelopamento profissional</p>
                    <p style="font-size: 0.9rem; color: var(--gray); margin-top: 10px;">Todas as marcas</p>
                </div>
                <div class="price-card">
                    <h3>Máquinas</h3>
                    <div class="price-from">A PARTIR DE</div>
                    <div class="price">400</div>
                    <p>Proteção e acabamento</p>
                    <p style="font-size: 0.9rem; color: var(--gray); margin-top: 10px;">Lavadora e secadora</p>
                </div>
            </div>
            <p style="text-align: center; margin-top: 3rem; color: var(--primary); font-weight: 600;">
                ⚡ Orçamento personalizado por WhatsApp • Pagamento facilitado • Garantia de 1 ano
            </p>
        </div>
    </section>

    <!-- Depoimentos -->
    <section id="depoimentos">
        <div class="container">
            <div class="section-title">
                <h2>Depoimentos Reais</h2>
                <p>A satisfação dos nossos clientes comprova a qualidade</p>
            </div>
            <div class="testimonials-container">
                <div class="testimonial-card">
                    <div class="testimonial-rating">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <div class="testimonial-text">
                        "Minha geladeira de 10 anos ficou nova! O trabalho foi impecável, rápido e sem sujeira. Super recomendo!"
                    </div>
                    <div class="testimonial-author">— Sandra Oliveira, Vila Madalena</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-rating">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <div class="testimonial-text">
                        "Escolhi o preto fosco e ficou perfeito! O acabamento é de primeira e o atendimento foi excelente."
                    </div>
                    <div class="testimonial-author">— Nair Santos, Moema</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-rating">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <div class="testimonial-text">
                        "Transformou minha cozinha inteira! Fogão, geladeira e micro-ondas ficaram com cara de novo. Vale cada centavo!"
                    </div>
                    <div class="testimonial-author">— José Carlos, Tatuapé</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Vantagens -->
    <section id="vantagens" style="background: linear-gradient(135deg, #f8fafc 0%, #edf2f7 100%);">
        <div class="container">
            <div class="section-title">
                <h2>Por que escolher a WILLSU?</h2>
                <p>Diferenciais que garantem a melhor experiência</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-shield-alt"></i></div>
                    <div class="service-content">
                        <h3>Técnica Exclusiva</h3>
                        <p>Impede o retorno da cor antiga e garante durabilidade por anos com nossa fórmula patenteada.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-spray-can"></i></div>
                    <div class="service-content">
                        <h3>Acabamento Perfeito</h3>
                        <p>Serviço limpo, sem cheiro forte ou bagunça. Seu ambiente fica intacto e organizado.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-truck"></i></div>
                    <div class="service-content">
                        <h3>Atendimento Local</h3>
                        <p>Vamos até você em toda Grande São Paulo. Atendemos em domicílio com agilidade.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-bolt"></i></div>
                    <div class="service-content">
                        <h3>Serviço Express</h3>
                        <p>Concluímos em 2-3 horas. Transformação rápida sem comprometer a qualidade.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-credit-card"></i></div>
                    <div class="service-content">
                        <h3>Pagamento Flexível</h3>
                        <p>PIX, cartão (débito/crédito), dinheiro. Parcelamos em 12x com a taxa da operadora do cartão.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon"><i class="fas fa-award"></i></div>
                    <div class="service-content">
                        <h3>Garantia Total</h3>
                        <p>1 ano de garantia em todos os serviços. Referência em qualidade e acabamento.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Cobertura -->
    <section id="cobertura">
        <div class="container">
            <div class="section-title">
                <h2>Área de Atuação</h2>
                <p>Atendemos em São Paulo capital e toda região metropolitana</p>
            </div>
            <div class="coverage-grid">
                <div class="city-card">São Paulo Capital</div>
                <div class="city-card">Osasco</div>
                <div class="city-card">Barueri</div>
                <div class="city-card">Itapevi</div>
                <div class="city-card">Cotia</div>
                <div class="city-card">Carapicuíba</div>
                <div class="city-card">Embu das Artes</div>
                <div class="city-card">Jandira</div>
                <div class="city-card">Taboão da Serra</div>
                <div class="city-card">Santo André</div>
                <div class="city-card">Diadema</div>
                <div class="city-card">Guarulhos</div>
                <div class="city-card">São Bernardo</div>
                <div class="city-card">Mauá</div>
                <div class="city-card">Ferraz de Vasconcelos</div>
                <div class="city-card">Itaquaquecetuba</div>
            </div>
        </div>
    </section>

    <!-- Sobre -->
    <section id="sobre" style="background: linear-gradient(135deg, #f0f7ff 0%, #e6f0ff 100%);">
        <div class="container">
            <div class="section-title">
                <h2>Sobre a WILLSU</h2>
                <p>Excelência em restauração e envelopamento</p>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3><i class="fas fa-bullseye"></i> Nossa Missão</h3>
                    <p>A <strong>WILLSU</strong> nasceu com a missão de revolucionar o mercado de restauração de eletrodomésticos e móveis através de técnicas modernas de envelopamento premium.</p>
                    <p>Somos referência na Grande São Paulo pelo <strong>capricho, profissionalismo e acabamento impecável</strong> que entregamos em cada projeto.</p>
                    
                    <h3 style="margin-top: 2rem;"><i class="fas fa-chart-line"></i> Nossa Trajetória</h3>
                    <p>Com mais de <strong>8 anos de experiência</strong>, já transformamos centenas de lares e estabelecimentos comerciais, sempre priorizando a satisfação total dos nossos clientes.</p>
                    <p>Nossa equipe é formada por <strong>profissionais especializados</strong> que dominam as mais modernas técnicas de aplicação e acabamento.</p>
                    
                    <h3 style="margin-top: 2rem;"><i class="fas fa-handshake"></i> Nosso Compromisso</h3>
                    <p>Acreditamos que <strong>renovar é melhor que substituir</strong>. Por isso, oferecemos uma solução econômica, ecológica e de altíssima qualidade para quem busca modernidade sem desperdício.</p>
                    <p><strong>Seu eletrodoméstico não precisa ser trocado. Ele precisa da WILLSU.</strong></p>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA -->
    <section class="cta">
        <div class="container">
            <div class="cta-content">
                <h2>Pronto para transformar sua casa?</h2>
                <p>Solicite um orçamento gratuito e descubra como podemos renovar seus eletrodomésticos e móveis com acabamento premium.</p>
                <a href="https://wa.me/5511983357198?text=Olá%20WILLSU!%20Gostaria%20de%20solicitar%20um%20orçamento%20gratuito%20para%20transformação%20de%20eletrodomésticos." 
                   class="btn-whatsapp-cta"
                   target="_blank"
                   aria-label="Falar no WhatsApp">
                    <i class="fab fa-whatsapp"></i> FALAR NO WHATSAPP AGORA
                </a>
                <p style="margin-top: 2rem; font-size: 1rem; opacity: 0.9;">
                    <i class="fas fa-clock"></i> Atendimento: Segunda a Sábado, 8h às 19h
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contato">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Contato Direto</h3>
                    <ul>
                        <li><i class="fab fa-whatsapp"></i> <a href="https://wa.me/5511983357198" target="_blank">(11) 98335-7198</a></li>
                        <li><i class="fas fa-phone"></i> (11) 98335-7198</li>
                        <li><i class="fas fa-envelope"></i> <a href="mailto:willsu.envelopamento@gmail.com">willsu.envelopamento@gmail.com</a></li>
                        <li><i class="fas fa-map-marker-alt"></i> São Paulo - SP e Região Metropolitana</li>
                        <li><i class="fas fa-clock"></i> Seg-Sáb: 8h às 19h</li>
                    </ul>
                    <div class="social-icons">
                        <a href="https://www.instagram.com/willsu.envelopamento/" target="_blank" aria-label="Instagram">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="https://www.facebook.com/willsu.envelopamento" target="_blank" aria-label="Facebook">
                            <i class="fab fa-facebook"></i>
                        </a>
                        <a href="https://wa.me/5511983357198" target="_blank" aria-label="WhatsApp">
                            <i class="fab fa-whatsapp"></i>
                        </a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Nossos Serviços</h3>
                    <ul>
                        <li><i class="fas fa-chevron-right"></i> <a href="#servicos">Envelopamento Premium</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#servicos">Restauração Completa</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#servicos">Solução Sustentável</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#servicos">Transformação de Móveis</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#servicos">Envelopamento de Cozinhas</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Links Rápidos</h3>
                    <ul>
                        <li><i class="fas fa-chevron-right"></i> <a href="#precos">Tabela de Preços</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#depoimentos">Depoimentos</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#cobertura">Cidades Atendidas</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#sobre">Sobre a Empresa</a></li>
                        <li><i class="fas fa-chevron-right"></i> <a href="#vantagens">Nossas Vantagens</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2024 <strong>WILLSU - Restauração e Envelopamento Premium</strong>. Todos os direitos reservados.</p>
                <p>CNPJ: XX.XXX.XXX/XXXX-XX • São Paulo - SP</p>
            </div>
            <div class="privacy-link">
                <a href="https://wmwilliansmiranda-jpg.github.io/willsu-sp.github/" target="_blank">
                    <i class="fas fa-shield-alt"></i> Política de Privacidade e Termos de Uso
                </a>
            </div>
        </div>
    </footer>

    <!-- WhatsApp Float -->
    <a href="https://wa.me/5511983357198?text=Olá%20WILLSU!%20Gostaria%20de%20solicitar%20um%20orçamento%20gratuito." 
       class="whatsapp-float" 
       target="_blank"
       aria-label="Falar no WhatsApp">
        <i class="fab fa-whatsapp"></i>
        <div class="whatsapp-badge">Online</div>
    </a>

    <script>
        // Menu Mobile
        const mobileMenu = document.getElementById('mobileMenu');
        const navLinks = document.getElementById('navLinks');
        
        mobileMenu.addEventListener('click', function() {
            navLinks.classList.toggle('active');
            mobileMenu.innerHTML = navLinks.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Fechar menu ao clicar em um link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
                mobileMenu.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });
        
        // Fechar menu ao clicar fora
        document.addEventListener('click', (e) => {
            if (!navLinks.contains(e.target) && !mobileMenu.contains(e.target)) {
                navLinks.classList.remove('active');
                mobileMenu.innerHTML = '<i class="fas fa-bars"></i>';
            }
        });
        
        // Scroll suave melhorado
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const target = document.querySelector(targetId);
                if (target) {
                    // Fechar menu mobile se aberto
                    if (navLinks.classList.contains('active')) {
                        navLinks.classList.remove('active');
                        mobileMenu.innerHTML = '<i class="fas fa-bars"></i>';
                    }
                    
                    // Scroll suave
                    window.scrollTo({
                        top: target.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Adicionar classe active na navegação conforme scroll
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('section[id]');
            const scrollPos = window.scrollY + 100;
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                const sectionId = section.getAttribute('id');
                
                if (scrollPos >= sectionTop && scrollPos < sectionTop + sectionHeight) {
                    document.querySelectorAll('.nav-links a').forEach(link => {
                        link.classList.remove('active');
                        if (link.getAttribute('href') === `#${sectionId}`) {
                            link.classList.add('active');
                        }
                    });
                }
            });
        });
        
        // Efeito de revelação ao scroll
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };
        
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);
        
        // Observar elementos para animação
        document.querySelectorAll('.service-card, .price-card, .testimonial-card, .city-card').forEach(el => {
            el.style.opacity = '0';
            el.style.transform = 'translateY(30px)';
            el.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            observer.observe(el);
        });
        
        // WhatsApp Tracking
        document.querySelectorAll('a[href*="whatsapp"]').forEach(link => {
            link.addEventListener('click', function() {
                gtag('event', 'conversion', {
                    'send_to': 'AW-17709030845/xxxxx',
                    'value': 1.0,
                    'currency': 'BRL'
                });
            });
        });
        
        // Loader
        window.addEventListener('load', () => {
            document.body.style.opacity = '0';
            document.body.style.transition = 'opacity 0.3s';
            setTimeout(() => {
                document.body.style.opacity = '1';
            }, 100);
        });
    </script>
</body>
</html>

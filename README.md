index.html

<!DOCTYPE html>
<html lang="pt-BR">
<head><!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=AW-17709030845"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'AW-17709030845');
</script>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
            --primary: #2c3e50;
            --secondary: #3498db;
            --accent: #e74c3c;
            --whatsapp: #25D366;
            --light: #ecf0f1;
            --dark: #2c3e50;
            --success: #27ae60;
        }

        body {
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
            overflow-x: hidden;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        /* HEADER MOBILE FIRST */
        header {
            background: var(--primary);
            color: white;
            padding: 1rem 0;
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.4rem;
            font-weight: bold;
            color: white;
        }

        .logo span {
            color: var(--secondary);
        }

        .mobile-menu {
            font-size: 1.5rem;
            cursor: pointer;
            color: white;
        }

        .nav-links {
            display: none;
            position: absolute;
            top: 100%;
            left: 0;
            right: 0;
            background: var(--primary);
            flex-direction: column;
            padding: 1rem;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        .nav-links.active {
            display: flex;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            padding: 0.8rem 1rem;
            display: block;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            transition: background 0.3s;
        }

        .nav-links a:hover {
            background: rgba(255,255,255,0.1);
        }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            padding: 6rem 0 3rem;
            text-align: center;
            margin-top: 60px;
        }

        .hero h1 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            line-height: 1.3;
        }

        .hero p {
            font-size: 1rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .btn {
            display: inline-block;
            background: var(--accent);
            color: white;
            padding: 14px 28px;
            text-decoration: none;
            border-radius: 8px;
            font-weight: bold;
            font-size: 1rem;
            transition: all 0.3s;
            border: none;
        }

        .btn-whatsapp {
            background: var(--whatsapp);
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        /* SECTIONS */
        section {
            padding: 3rem 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 2rem;
        }

        .section-title h2 {
            font-size: 1.8rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .section-title p {
            color: #666;
            font-size: 1rem;
        }

        /* SERVICES */
        .services-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        .service-card {
            background: white;
            border-radius: 12px;
            padding: 1.5rem;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
        }

        .service-icon {
            background: var(--primary);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }

        .service-content h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .service-content ul {
            list-style: none;
        }

        .service-content li {
            margin-bottom: 0.5rem;
            padding-left: 1.5rem;
            position: relative;
        }

        .service-content li:before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--success);
            font-weight: bold;
        }

        /* PRICING */
        .pricing-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        .price-card {
            background: white;
            border-radius: 12px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            border: 2px solid transparent;
            transition: all 0.3s;
        }

        .price-card:hover {
            border-color: var(--secondary);
        }

        .price-card h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .price {
            font-size: 2rem;
            font-weight: bold;
            color: var(--accent);
            margin: 1rem 0;
        }

        /* TESTIMONIALS */
        .testimonials-container {
            display: grid;
            grid-template-columns: 1fr;
            gap: 1.5rem;
        }

        .testimonial-card {
            background: white;
            border-radius: 12px;
            padding: 1.5rem;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            position: relative;
        }

        .testimonial-card:before {
            content: '"';
            font-size: 3rem;
            color: var(--secondary);
            position: absolute;
            top: 10px;
            left: 15px;
            opacity: 0.3;
        }

        .testimonial-text {
            font-style: italic;
            margin-bottom: 1rem;
            padding-left: 1rem;
        }

        .testimonial-author {
            font-weight: bold;
            color: var(--primary);
            text-align: right;
        }

        /* COVERAGE */
        .coverage-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1rem;
        }

        .city-card {
            background: white;
            border-radius: 8px;
            padding: 1rem;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0,0,0,0.1);
            font-size: 0.9rem;
        }

        /* ABOUT */
        .about-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
        }

        .about-text h3 {
            color: var(--primary);
            margin-bottom: 1rem;
            font-size: 1.4rem;
        }

        .about-text p {
            margin-bottom: 1rem;
        }

        /* CTA */
        .cta {
            background: linear-gradient(135deg, var(--primary) 0%, var(--secondary) 100%);
            color: white;
            text-align: center;
            padding: 3rem 1rem;
        }

        .cta h2 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
        }

        .cta p {
            font-size: 1rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        /* FOOTER */
        footer {
            background: var(--dark);
            color: white;
            padding: 2rem 0 1rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-column h3 {
            color: var(--secondary);
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        .footer-column ul {
            list-style: none;
        }

        .footer-column li {
            margin-bottom: 0.5rem;
        }

        .footer-column a {
            color: #ddd;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-column a:hover {
            color: var(--secondary);
        }

        .copyright {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
            color: #aaa;
        }

        .privacy-link {
            text-align: center;
            margin-top: 1rem;
        }

        .privacy-link a {
            color: #aaa;
            text-decoration: none;
            font-size: 0.9rem;
            transition: color 0.3s;
        }

        .privacy-link a:hover {
            color: var(--secondary);
        }

        /* WHATSAPP FLOAT */
        .whatsapp-float {
            position: fixed;
            bottom: 20px;
            right: 20px;
            width: 60px;
            height: 60px;
            background: var(--whatsapp);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            box-shadow: 0 4px 20px rgba(0,0,0,0.3);
            z-index: 1000;
            text-decoration: none;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        /* DESKTOP STYLES */
        @media (min-width: 768px) {
            .container {
                padding: 0 20px;
            }

            .mobile-menu {
                display: none;
            }

            .nav-links {
                display: flex;
                position: static;
                flex-direction: row;
                background: none;
                box-shadow: none;
                padding: 0;
            }

            .nav-links a {
                padding: 0.5rem 1rem;
                border-bottom: none;
            }

            .hero {
                padding: 8rem 0 4rem;
                margin-top: 0;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.2rem;
            }

            .services-grid {
                grid-template-columns: repeat(3, 1fr);
            }

            .pricing-grid {
                grid-template-columns: repeat(4, 1fr);
            }

            .testimonials-container {
                grid-template-columns: repeat(3, 1fr);
            }

            .coverage-grid {
                grid-template-columns: repeat(4, 1fr);
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .footer-content {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        /* LARGE DESKTOP */
        @media (min-width: 1200px) {
            .hero h1 {
                font-size: 3rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">WILL<span>SU</span></div>
                <div class="mobile-menu">☰</div>
                <nav class="nav-links">
                    <a href="#servicos">Serviços</a>
                    <a href="#precos">Preços</a>
                    <a href="#depoimentos">Depoimentos</a>
                    <a href="#cobertura">Área de Atuação</a>
                    <a href="#sobre">Sobre</a>
                    <a href="#contato">Contato</a>
                </nav>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
   <h1>Transformamos eletrodomésticos e móveis com adesivo e acabamento premium</h1>
<p>Deixe seus eletros como novos com técnica exclusiva e durabilidade garantida.</p>

<a href="https://wa.me/5511983357198" 
   style="
     display: inline-block;
     background-color: #25D366;
     color: white;
     padding: 12px 20px;
     border-radius: 8px;
     font-size: 18px;
     text-decoration: none;
     font-weight: bold;
     margin-top: 10px;
   ">
  Solicitar Orçamento
</a>

<p style="margin-top: 10px; color: #444;">
  Entre em contato somente se houver real intenção de prosseguir com o orçamento.
</p>


<p class="observacao">Entre em contato somente se houver real intenção de prosseguir com o orçamento.</p>

            
            <p style="margin-top: 1rem; font-size: 0.9rem; opacity: 0.8;">
                Entre em contato somente se houver real intenção de prosseguir
            </p>
        </div>
    </section>

    <!-- Serviços -->
    <section id="servicos">
        <div class="container">
            <div class="section-title">
                <h2>Nossos Serviços</h2>
                <p>Soluções completas de restauração e envelopamento</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">✨</div>
                    <div class="service-content">
                        <h3>Envelopamento Premium</h3>
                        <p>Cores modernas e alta durabilidade para:</p>
                        <ul>
                            <li>Geladeiras</li>
                            <li>Fogões</li>
                            <li>Micro-ondas</li>
                            <li>Máquinas de lavar</li>
                            <li>Móveis em geral</li>
                        </ul>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">🔧</div>
                    <div class="service-content">
                        <h3>Restauração Completa</h3>
                        <p>Recuperamos a aparência original:</p>
                        <ul>
                            <li>Remoção de ferrugem</li>
                            <li>Restauração de superfícies</li>
                            <li>Correção de amarelado</li>
                            <li>Troca de componentes</li>
                            <li>Técnica exclusiva</li>
                        </ul>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">♻️</div>
                    <div class="service-content">
                        <h3>Sustentabilidade</h3>
                        <p>Renove ao invés de trocar:</p>
                        <ul>
                            <li>Mais barato</li>
                            <li>Mais moderno</li>
                            <li>Mais ecológico</li>
                            <li>Reduza descartes</li>
                            <li>Economize recursos</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Preços -->
    <section id="precos" style="background-color: #f0f5ff;">
        <div class="container">
            <div class="section-title">
                <h2>Nossos Preços</h2>
                <p>Valores iniciais - orçamento personalizado</p>
            </div>
            <div class="pricing-grid">
                <div class="price-card">
                    <h3>Geladeiras</h3>
                    <div class="price">A partir de R$ 500,00</div>
                    <p>Transformação completa</p>
                </div>
                <div class="price-card">
                    <h3>Fogões</h3>
                    <div class="price">A partir de R$ 300,00</div>
                    <p>Renovação estética</p>
                </div>
                <div class="price-card">
                    <h3>Micro-ondas</h3>
                    <div class="price">A partir de R$ 180,00</div>
                    <p>Envelopamento profissional</p>
                </div>
                <div class="price-card">
                    <h3>Máquinas</h3>
                    <div class="price">A partir de R$ 400,00</div>
                    <p>Proteção e acabamento</p>
                </div>
            </div>
            <p style="text-align: center; margin-top: 2rem; color: #666;">
                * Valor final personalizado conforme aparelho
            </p>
        </div>
    </section>

    <!-- Depoimentos -->
    <section id="depoimentos">
        <div class="container">
            <div class="section-title">
                <h2>Depoimentos</h2>
                <p>O que nossos clientes dizem</p>
            </div>
            <div class="testimonials-container">
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        Minha geladeira ficou nova! Atendimento rápido e profissional.
                    </div>
                    <div class="testimonial-author">— Sandra</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        O preto fosco ficou lindo. Trabalho impecável!
                    </div>
                    <div class="testimonial-author">— Nair</div>
                </div>
                <div class="testimonial-card">
                    <div class="testimonial-text">
                        Transformou minha geladeira antiga. Perfeito!
                    </div>
                    <div class="testimonial-author">— José</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Vantagens -->
    <section id="vantagens" style="background-color: #f9f9f9;">
        <div class="container">
            <div class="section-title">
                <h2>Por que escolher a WILLSU?</h2>
                <p>Diferenciais que fazem a diferença</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-content">
                        <h3>🔒 Técnica Exclusiva</h3>
                        <p>Impede o retorno da cor antiga e garante durabilidade por anos.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-content">
                        <h3>🧼 Acabamento Limpo</h3>
                        <p>Serviço sem sujeira, cheiro ou bagunça no seu ambiente.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-content">
                        <h3>🚚 Atendimento Local</h3>
                        <p>Vamos até você em toda Grande São Paulo.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-content">
                        <h3>⚡ Serviço Rápido</h3>
                        <p>Concluímos em apenas 2 a 3 horas.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-content">
                        <h3>💳 Pagamento Facilitado</h3>
                        <p>PIX, cartão, débito e crédito.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-content">
                        <h3>🏆 Profissionalismo</h3>
                        <p>Referência em qualidade e acabamento.</p>
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
            </div>
        </div>
    </section>

    <!-- Sobre -->
    <section id="sobre" style="background-color: #f0f5ff;">
        <div class="container">
            <div class="section-title">
                <h2>Sobre a WILLSU</h2>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>Nossa Missão</h3>
                    <p>A WILLSU nasceu com a missão de transformar eletrodomésticos e móveis usando técnicas modernas de envelopamento e restauração.</p>
                    <p>Atendemos centenas de clientes por mês e somos referência na Grande São Paulo pelo capricho, profissionalismo e acabamento impecável.</p>
                    <p>Aqui, seu eletrodoméstico não precisa ser trocado. Ele precisa da WILLSU.</p>
                    <p>Bem-vindo à Willsu, onde transformamos seus eletrodomésticos antigos em peças modernas, elegantes e duráveis. Nosso objetivo é entregar qualidade, beleza e resistência em cada serviço.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA -->
    <section class="cta">
        <div class="container">
            <h2>Pronto para transformar?</h2>
            <p>Solicite um orçamento sem compromisso</p>
            <a href="https://wa.me/5511983357198?text=Olá! Gostaria de solicitar um orçamento" class="btn btn-whatsapp">
                <i class="fab fa-whatsapp"></i> Falar no WhatsApp
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contato">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Contato</h3>
                    <ul>
                        <li><i class="fab fa-whatsapp"></i> (11) 98335-7198</li>
                        <li><i class="fas fa-envelope"></i> willsu.envelopamento@gmail.com</li>
                        <li><i class="fas fa-map-marker-alt"></i> São Paulo e Região Metropolitana</li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Serviços</h3>
                    <ul>
                        <li><a href="#servicos">Envelopamento</a></li>
                        <li><a href="#servicos">Restauração</a></li>
                        <li><a href="#servicos">Sustentabilidade</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Links</h3>
                    <ul>
                        <li><a href="#precos">Preços</a></li>
                        <li><a href="#depoimentos">Depoimentos</a></li>
                        <li><a href="#cobertura">Área de Atuação</a></li>
                        <li><a href="#sobre">Sobre Nós</a></li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                &copy; 2023 WILLSU - Todos os direitos reservados.
            </div>
            <div class="privacy-link">
                <a href="https://wmwilliansmiranda-jpg.github.io/willsu-sp.github/" target="_blank">Política de Privacidade</a>
            </div>
        </div>
    </footer>

    <!-- WhatsApp Float -->
    <a href="https://wa.me/5511983357198?text=Olá! Gostaria de solicitar um orçamento" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <script>
        // Menu Mobile
        document.querySelector('.mobile-menu').addEventListener('click', function() {
            document.querySelector('.nav-links').classList.toggle('active');
        });

        // Fechar menu ao clicar em um link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                document.querySelector('.nav-links').classList.remove('active');
            });
        });

        // Scroll suave
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>

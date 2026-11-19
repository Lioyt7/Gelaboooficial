[Pagina Gelaboo.html](https://github.com/user-attachments/files/35060571/Pagina.Gelaboo.html)
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gelaboo | Gelatinas en Vasitos</title>
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@500;700&family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-dark: #070709;
            --bg-card: #111116;
            --bg-card-hover: #17171f;
            --neon-green: #39ff14;
            --neon-red: #ff1e27;
            --text-main: #f5f5f7;
            --text-muted: #a1a1aa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            overflow-x: hidden;
        }

        h1, h2, h3, .brand-font {
            font-family: 'Fredoka', sans-serif;
            letter-spacing: 0.5px;
        }

        /* NAVEGACIÓN */
        header {
            position: sticky;
            top: 0;
            z-index: 100;
            background: rgba(7, 7, 9, 0.9);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(57, 255, 20, 0.25);
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .nav-brand {
            display: flex;
            align-items: center;
            gap: 12px;
            text-decoration: none;
        }

        .nav-brand img {
            height: 45px;
            width: auto;
        }

        .nav-brand span {
            font-family: 'Fredoka', sans-serif;
            font-size: 1.6rem;
            font-weight: 700;
            color: var(--neon-green);
            text-shadow: 0 0 10px rgba(57, 255, 20, 0.4);
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 28px;
        }

        nav a {
            color: var(--text-main);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--neon-green);
        }

        /* HERO / PORTADA */
        .hero {
            padding: 70px 5% 80px;
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            align-items: center;
            gap: 50px;
        }

        .hero-badge {
            display: inline-block;
            background: rgba(255, 30, 39, 0.15);
            color: var(--neon-red);
            border: 1px solid var(--neon-red);
            padding: 6px 16px;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 700;
            margin-bottom: 18px;
            box-shadow: 0 0 15px rgba(255, 30, 39, 0.25);
        }

        .hero h1 {
            font-size: 3.6rem;
            line-height: 1.1;
            margin-bottom: 20px;
        }

        .hero h1 span.green {
            color: var(--neon-green);
            text-shadow: 0 0 20px rgba(57, 255, 20, 0.35);
        }

        .hero h1 span.red {
            color: var(--neon-red);
            text-shadow: 0 0 20px rgba(255, 30, 39, 0.35);
        }

        .hero p {
            color: var(--text-muted);
            font-size: 1.1rem;
            margin-bottom: 30px;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn-primary {
            background: var(--neon-green);
            color: #050505;
            padding: 14px 30px;
            border-radius: 12px;
            font-weight: 700;
            text-decoration: none;
            box-shadow: 0 0 20px rgba(57, 255, 20, 0.4);
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 0 30px rgba(57, 255, 20, 0.7);
        }

        .btn-secondary {
            background: transparent;
            color: var(--text-main);
            border: 2px solid var(--neon-red);
            padding: 12px 28px;
            border-radius: 12px;
            font-weight: 600;
            text-decoration: none;
            transition: background 0.2s;
        }

        .btn-secondary:hover {
            background: rgba(255, 30, 39, 0.15);
        }

        .hero-visual {
            text-align: center;
            position: relative;
        }

        .hero-logo {
            max-width: 100%;
            width: 440px;
            filter: drop-shadow(0 0 25px rgba(57, 255, 20, 0.25));
            transition: transform 0.4s ease;
        }

        .hero-logo:hover {
            transform: scale(1.03);
        }

        /* SECCIÓN PROPUESTA DE VALOR */
        .value-section {
            background: #0c0c10;
            border-top: 1px solid rgba(255, 30, 39, 0.25);
            border-bottom: 1px solid rgba(57, 255, 20, 0.25);
            padding: 80px 5%;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 55px;
        }

        .section-header h2 {
            font-size: 2.5rem;
            margin-bottom: 12px;
        }

        .section-header p {
            color: var(--text-muted);
        }

        .value-grid {
            display: grid;
            grid-template-columns: 1.1fr 0.9fr;
            gap: 40px;
            align-items: center;
        }

        .main-showcase-img {
            width: 100%;
            border-radius: 20px;
            border: 2px solid var(--neon-green);
            box-shadow: 0 0 30px rgba(57, 255, 20, 0.2);
            display: block;
        }

        .value-cards {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .value-card {
            background: var(--bg-card);
            padding: 25px;
            border-radius: 16px;
            border-left: 4px solid var(--neon-red);
        }

        .value-card.green-border {
            border-left-color: var(--neon-green);
        }

        .value-card h3 {
            font-size: 1.3rem;
            margin-bottom: 8px;
            color: #fff;
        }

        .value-card p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        /* SECCIÓN PRODUCTOS */
        .products-section {
            padding: 90px 5%;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 30px;
        }

        .product-card {
            background: var(--bg-card);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 22px;
            overflow: hidden;
            transition: transform 0.3s, border-color 0.3s, box-shadow 0.3s;
            display: flex;
            flex-direction: column;
        }

        .product-card:hover {
            transform: translateY(-8px);
            border-color: var(--neon-green);
            box-shadow: 0 12px 35px rgba(57, 255, 20, 0.15);
        }

        .product-card.red-accent:hover {
            border-color: var(--neon-red);
            box-shadow: 0 12px 35px rgba(255, 30, 39, 0.18);
        }

        .product-img-box {
            width: 100%;
            height: 240px;
            background: #181820;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            border-bottom: 1px solid rgba(255, 255, 255, 0.06);
        }

        .product-img-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .ratio-tag {
            position: absolute;
            top: 14px;
            right: 14px;
            background: rgba(7, 7, 9, 0.85);
            color: var(--neon-green);
            border: 1px solid var(--neon-green);
            padding: 4px 12px;
            border-radius: 50px;
            font-size: 0.75rem;
            font-weight: 700;
        }

        .product-body {
            padding: 25px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .product-body h3 {
            font-size: 1.45rem;
            margin-bottom: 10px;
        }

        .product-body p {
            color: var(--text-muted);
            font-size: 0.92rem;
            margin-bottom: 22px;
        }

        .product-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 15px;
            border-top: 1px solid rgba(255, 255, 255, 0.08);
        }

        .price {
            font-family: 'Fredoka', sans-serif;
            font-size: 1.6rem;
            font-weight: 700;
            color: var(--neon-green);
        }

        .price small {
            display: block;
            font-family: 'Poppins', sans-serif;
            font-size: 0.72rem;
            font-weight: 400;
            color: var(--text-muted);
        }

        .btn-card {
            background: var(--neon-red);
            color: #fff;
            padding: 9px 18px;
            border-radius: 10px;
            text-decoration: none;
            font-size: 0.88rem;
            font-weight: 600;
            transition: opacity 0.2s;
        }

        .btn-card:hover {
            opacity: 0.85;
        }

        /* SECCIÓN CONTACTO / CTA */
        .cta-section {
            padding: 80px 5% 100px;
        }

        .cta-box {
            max-width: 1050px;
            margin: 0 auto;
            background: linear-gradient(145deg, #121218, #0b0b0e);
            border: 2px solid var(--neon-red);
            box-shadow: 0 0 40px rgba(255, 30, 39, 0.15);
            border-radius: 26px;
            padding: 50px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 45px;
            align-items: center;
        }

        .cta-info h2 {
            font-size: 2.4rem;
            margin-bottom: 15px;
        }

        .cta-info h2 span {
            color: var(--neon-green);
        }

        .cta-info p {
            color: var(--text-muted);
            margin-bottom: 25px;
        }

        .contact-badges {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .contact-item {
            background: rgba(255, 255, 255, 0.04);
            padding: 12px 18px;
            border-radius: 12px;
            font-size: 0.95rem;
            border-left: 3px solid var(--neon-green);
        }

        form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        input, select, textarea {
            width: 100%;
            background: #070709;
            border: 1px solid rgba(255, 255, 255, 0.15);
            color: #fff;
            padding: 14px 16px;
            border-radius: 12px;
            font-family: 'Poppins', sans-serif;
            font-size: 0.95rem;
            outline: none;
            transition: border-color 0.3s;
        }

        input:focus, select:focus, textarea:focus {
            border-color: var(--neon-green);
        }

        button[type="submit"] {
            background: var(--neon-green);
            color: #050505;
            border: none;
            padding: 15px;
            border-radius: 12px;
            font-family: 'Fredoka', sans-serif;
            font-size: 1.15rem;
            font-weight: 700;
            cursor: pointer;
            box-shadow: 0 0 20px rgba(57, 255, 20, 0.35);
            transition: transform 0.2s, box-shadow 0.2s;
        }

        button[type="submit"]:hover {
            transform: translateY(-2px);
            box-shadow: 0 0 30px rgba(57, 255, 20, 0.6);
        }

        footer {
            text-align: center;
            padding: 30px 5%;
            border-top: 1px solid rgba(255, 255, 255, 0.08);
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* RESPONSIVE PARA CELULARES */
        @media (max-width: 900px) {
            .hero, .value-grid, .products-grid, .cta-box {
                grid-template-columns: 1fr;
            }
            .hero {
                text-align: center;
                padding-top: 40px;
            }
            .hero h1 {
                font-size: 2.6rem;
            }
            .hero-buttons {
                justify-content: center;
            }
            nav ul {
                display: none;
            }
            .cta-box {
                padding: 30px 22px;
            }
        }
    </style>
</head>
<body>

    <!-- BARRA DE NAVEGACIÓN -->
    <header>
        <a href="#inicio" class="nav-brand">
            <img src="Gelaboo_ Monstruos Navideños y Gelatinas.png" alt="Logo Gelaboo">
            <span>GELABOO</span>
        </a>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#propuesta">Propuesta</a></li>
                <li><a href="#productos">Productos</a></li>
                <li><a href="#contacto">Pedir Ahora</a></li>
            </ul>
        </nav>
    </header>

    <!-- SECCIÓN 1: INICIO / PRESENTACIÓN -->
    <section id="inicio" class="hero">
        <div class="hero-text">
            <span class="hero-badge">★ EDICIÓN MONSTRUOSA & NAVIDEÑA ★</span>
            <h1>El postre más <span class="green">vibrante</span> y <span class="red">cremoso</span> en vasito.</h1>
            <p>
                En <strong>Gelaboo</strong> reinventamos la gelatina tradicional con sabores intensos, 
                estética divertida y nuestra fórmula exacta: <strong>90% gelatina fresca + 10% glaseado dulce de leche</strong> en vasitos listos para disfrutar.
            </p>
            <div class="hero-buttons">
                <a href="#productos" class="btn-primary">Ver Sabores y Precios</a>
                <a href="#contacto" class="btn-secondary">Hacer un Pedido</a>
            </div>
        </div>
        <div class="hero-visual">
            <!-- LOGO DEL EMPRENDIMIENTO -->
            <img src="Gelaboo_ Monstruos Navideños y Gelatinas.png" alt="Logo Oficial Gelaboo" class="hero-logo">
        </div>
    </section>

    <!-- SECCIÓN 2: PROPUESTA DE VALOR Y FOTO PRINCIPAL -->
    <section id="propuesta" class="value-section">
        <div class="container">
            <div class="section-header">
                <h2>¿Por qué elegir <span style="color: var(--neon-green);">Gelaboo</span>?</h2>
                <p>Combinamos sabor, practicidad y una presentación visual que roba miradas en cualquier mesa.</p>
            </div>

            <div class="value-grid">
                <div>
                    <!-- FOTO PRINCIPAL DE TUS GELATINAS -->
                    <img src="Fondo vertical gelaboo.png" alt="Vasitos de Gelatina Gelaboo 90/10" class="main-showcase-img">
                </div>
                <div class="value-cards">
                    <div class="value-card green-border">
                        <h3>⚡ Proporción Exacta 90% / 10%</h3>
                        <p>Cada vasito descartable lleva 90% de gelatina firme y refrescante, coronada con un 10% de glaseado cremoso de leche en la superficie.</p>
                    </div>
                    <div class="value-card">
                        <h3>🎄 Temática Única y Divertida</h3>
                        <p>Perfectas para fiestas, reuniones navideñas, cumpleaños o para darte un gusto diferente con colores llamativos.</p>
                    </div>
                    <div class="value-card green-border">
                        <h3>🥤 Formato Práctico e Higiénico</h3>
                        <p>Servidas en vasitos individuales listos para repartir sin complicaciones y mantener siempre su frescura.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN 3: 3 PRODUCTOS CON IMÁGENES Y PRECIOS REFERENCIALES -->
    <section id="productos" class="products-section">
        <div class="container">
            <div class="section-header">
                <h2>Nuestros <span style="color: var(--neon-red);">Productos Estrella</span></h2>
                <p>Elige tu favorito o arma tu combo para compartir. Precios referenciales sujetos a cantidad.</p>
            </div>

            <div class="products-grid">
                <!-- PRODUCTO 1 -->
                <article class="product-card red-accent">
                    <div class="product-img-box">
                        <span class="ratio-tag">90% Gelatina • 10% Leche</span>
                        <!-- REEMPLAZA ESTA RUTA CON TU FOTO 1 -->
                        <img src="foto fresa gelaboo.png" alt="Gelatina Roja Monstruosa">
                    </div>
                    <div class="product-body">
                        <div>
                            <h3>Rojo Monstruoso</h3>
                            <p>Intenso sabor a fresa en vasito individual, cubierto con nuestra capa superior de glaseado cremoso de leche.</p>
                        </div>
                        <div class="product-footer">
                            <div class="price">
                                S/ 2.00
                                <small>Precio referencial c/u</small>
                            </div>
                            <a href="#contacto" class="btn-card">Pedir</a>
                        </div>
                    </div>
                </article>

                <!-- PRODUCTO 2 -->
                <article class="product-card">
                    <div class="product-img-box">
                        <span class="ratio-tag">90% Gelatina • 10% Leche</span>
                        <!-- REEMPLAZA ESTA RUTA CON TU FOTO 2 -->
                        <img src="foto Manzana gelaboo.png" alt="Gelatina Verde Limon Monstruosa">
                    </div>
                    <div class="product-body">
                        <div>
                            <h3>Verde Limon Monstruoso</h3>
                            <p>Refrescante sabor a limón ácido equilibrado a la perfección con el toque dulce del 10% de glaseado lácteo arriba.</p>
                        </div>
                        <div class="product-footer">
                            <div class="price">
                                S/ 2.00
                                <small>Precio referencial c/u</small>
                            </div>
                            <a href="#contacto" class="btn-card">Pedir</a>
                        </div>
                    </div>
                </article>

                <!-- PRODUCTO 3 -->
                <article class="product-card red-accent">
                    <div class="product-img-box">
                        <span class="ratio-tag">Naranja Monstruoso</span>
                        <!-- REEMPLAZA ESTA RUTA CON TU FOTO 3 -->
                        <img src="foto Naranja gelaboo.png" alt="Naranja Monstruoso">
                    </div>
                    <div class="product-body">
                        <div>
                            <h3>Naranaja Monstruoso</h3>
                            <p>Refrescante sabor a Naranja con su glaseado de leche listo para eventos.</p>
                        </div>
                        <div class="product-footer">
                            <div class="price">
                                S/ 2.00
                                <small>Precio referencial pack</small>
                            </div>
                            <a href="#contacto" class="btn-card">Pedir</a>
                        </div>
                    </div>
                </article>

                <!-- PRODUCTO 4 -->
                <article class="product-card">
                    <div class="product-img-box">
                        <span class="ratio-tag">90% Gelatina • 10% Leche</span>
                        <!-- REEMPLAZA ESTA RUTA CON TU FOTO 2 -->
                        <img src="foto Chicle gelaboo.png" alt="Gelatina Azul Monstruosa">
                    </div>
                    <div class="product-body">
                        <div>
                            <h3>Azul Chicle Monstruoso</h3>
                            <p>Refrescante sabor a Chicle equilibrado a la perfección con el toque dulce del 10% de glaseado lácteo arriba.</p>
                        </div>
                        <div class="product-footer">
                            <div class="price">
                                S/ 2.00
                                <small>Precio referencial c/u</small>
                            </div>
                            <a href="#contacto" class="btn-card">Pedir</a>
                        </div>
                    </div>
                </article>

            </div>
        </div>
    </section>

    <!-- SECCIÓN 4: CONTACTO Y LLAMADA A LA ACCIÓN -->
    <section id="contacto" class="cta-section">
        <div class="cta-box">
            <div class="cta-info">
                <h2>¿Listo para probar <span>Gelaboo</span>?</h2>
                <p>Haz tu pedido para reuniones o antojos del día. Te respondemos al instante para coordinar tu entrega.</p>
                <div class="contact-badges">
                    <div class="contact-item"><strong>📱 WhatsApp Directo:</strong> +51 974 408 031 </div>
                    <div class="contact-item"><strong>📸 Instagram</strong> @Gelaboo.oficial</div>
                    <div class="contact-item"><strong>📍 Entregas:</strong> Venta directa y recojo previa coordinación</div>
                </div>
            </div>

            <form action="#" method="post">
                <input type="text" name="nombre" placeholder="Tu nombre completo" required>
                <input type="tel" name="whatsapp" placeholder="Tu número de WhatsApp" required>
                <select name="pedido">
                    <option value="rojo">Rojo Monstruoso (S/ 2.00 c/u)</option>
                    <option value="verde">Verde Limon Monstruoso (S/ 2.00 c/u)</option>
                    <option value="pack">Naranja Monstruoso (S/ 2.00)</option>
                    <option value="pack">Azul Chicle Monstruoso (S/ 2.00)</option>
                </select>
                <textarea name="detalles" rows="3" placeholder="Indica la cantidad de vasitos y fecha de entrega..."></textarea>
                <button type="submit">ENVIAR PEDIDO AHORA</button>
            </form>
        </div>
    </section>

    <footer>
        <p>© 2026 <strong>Gelaboo - Gelatinas en Vasitos</strong>. Todos los derechos reservados.</p>
    </footer>

</body>
</html>

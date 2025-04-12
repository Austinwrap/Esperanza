<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Esperanza - Handmade Mexican Treasures</title>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;700&family=Open+Sans:wght@400&display=swap" rel="stylesheet">
    <style>
        html, body {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
            overflow-x: hidden;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            background-color: #FFF0F5;
            color: #333;
            line-height: 1.8;
        }

        .navbar {
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 15px 20px;
            background: #FFFFFF;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .nav-links {
            display: flex;
            gap: 20px;
            list-style: none;
            margin: 0;
            padding: 0;
        }

        .nav-links a {
            text-decoration: none;
            color: #333;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.2rem;
            padding: 10px 15px;
            transition: color 0.3s ease, background 0.3s ease;
        }

        .nav-links a:hover {
            color: #E91E63;
            background: rgba(233, 30, 99, 0.05);
            border-radius: 5px;
        }

        .hero {
            min-height: 80vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            background: linear-gradient(rgba(255, 240, 245, 0.9), rgba(255, 240, 245, 0.9)), url('https://images.unsplash.com/photo-1614028674026-a65e31bfd27c?q=80&w=1920&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
        }

        .hero-content h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 3.5rem;
            color: #222;
            margin-bottom: 20px;
        }

        .hero-content p {
            font-size: 1.1rem;
            color: #444;
            max-width: 500px;
            margin: 0 auto 30px;
        }

        .cta-button {
            display: inline-block;
            padding: 12px 30px;
            background: #E91E63;
            color: #FFF;
            text-decoration: none;
            border-radius: 5px;
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.2rem;
            transition: background 0.3s ease, transform 0.3s ease;
        }

        .cta-button:hover {
            background: #C2185B;
            transform: translateY(-2px);
        }

        .shop {
            padding: 60px 15px;
            text-align: center;
            background: #FFF;
        }

        .shop h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2.8rem;
            color: #222;
            margin-bottom: 40px;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .product-card {
            background: #FFF0F5;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .product-card:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .product-card .icon {
            font-size: 3rem;
            margin-bottom: 15px;
            color: #E91E63;
        }

        .product-card h3 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 1.4rem;
            color: #222;
            margin-bottom: 10px;
        }

        .product-card p {
            font-size: 0.9rem;
            color: #555;
        }

        .about {
            padding: 60px 15px;
            text-align: center;
            background: #FFF0F5;
        }

        .about h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2.8rem;
            color: #222;
            margin-bottom: 20px;
        }

        .about p {
            max-width: 700px;
            margin: 0 auto;
            color: #444;
            font-size: 1rem;
        }

        .contact {
            padding: 60px 15px;
            text-align: center;
            background: #FFF;
        }

        .contact h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2.8rem;
            color: #222;
            margin-bottom: 20px;
        }

        .contact p {
            font-size: 1rem;
            color: #444;
            margin-bottom: 10px;
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #FFF0F5;
            color: #444;
            font-size: 0.9rem;
        }

        @media (max-width: 428px) {
            .navbar {
                padding: 10px;
            }

            .nav-links {
                flex-wrap: wrap;
                justify-content: center;
                gap: 10px;
            }

            .nav-links a {
                font-size: 1rem;
                padding: 8px 12px;
            }

            .hero-content h1 {
                font-size: 2.2rem;
            }

            .hero-content p {
                font-size: 0.95rem;
                padding: 0 15px;
            }

            .cta-button {
                padding: 10px 20px;
                font-size: 1rem;
            }

            .shop h2, .about h2, .contact h2 {
                font-size: 2rem;
            }

            .product-grid {
                grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
                gap: 15px;
            }

            .product-card .icon {
                font-size: 2.5rem;
            }

            .product-card h3 {
                font-size: 1.2rem;
            }

            .product-card p {
                font-size: 0.85rem;
            }
        }

        @media (min-width: 429px) and (max-width: 768px) {
            .product-grid {
                grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            }

            .hero-content h1 {
                font-size: 3rem;
            }

            .nav-links a {
                font-size: 1.1rem;
            }
        }

        @media (min-width: 769px) {
            .hero {
                min-height: 90vh;
            }

            .product-grid {
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            }

            .nav-links {
                gap: 25px;
            }

            .nav-links a {
                font-size: 1.3rem;
            }
        }
    </style>
</head>
<body>
    <nav class="navbar">
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#shop">Shop</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Esperanza</h1>
            <p>Handcrafted Mexican treasures made with heart and heritage.</p>
            <a href="#shop" class="cta-button">Explore Now</a>
        </div>
    </section>

    <section id="shop" class="shop">
        <h2>Our Collection</h2>
        <div class="product-grid">
            <div class="product-card">
                <div class="icon">💎</div>
                <h3>Earrings</h3>
                <p>Sparkling designs with artisan flair.</p>
            </div>
            <div class="product-card">
                <div class="icon">📿</div>
                <h3>Bracelets</h3>
                <p>Handwoven elegance for your wrist.</p>
            </div>
            <div class="product-card">
                <div class="icon">💍</div>
                <h3>Necklaces</h3>
                <p>Bold pieces with cultural charm.</p>
            </div>
            <div class="product-card">
                <div class="icon">⌚</div>
                <h3>Watches</h3>
                <p>Crafted timepieces with soul.</p>
            </div>
            <div class="product-card">
                <div class="icon">🧴</div>
                <h3>Hair Products</h3>
                <p>Natural care for radiant locks.</p>
            </div>
            <div class="product-card">
                <div class="icon">👁️‍🗨️</div>
                <h3>Eyelashes</h3>
                <p>Artisan lashes for stunning eyes.</p>
            </div>
            <div class="product-card">
                <div class="icon">💄</div>
                <h3>Makeup</h3>
                <p>Vibrant beauty with handmade care.</p>
            </div>
            <div class="product-card">
                <div class="icon">👗</div>
                <h3>Clothes</h3>
                <p>Fashion rooted in tradition.</p>
            </div>
        </div>
    </section>

    <section id="about" class="about">
        <h2>About Esperanza</h2>
        <p>Esperanza honors the artistry of Mexico. Every creation, from jewelry to clothing, is handmade by skilled artisans who weave love and tradition into their work. Our treasures bring elegance and culture to your everyday life.</p>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Email: info@esperanza.mx</p>
        <p>Instagram: @EsperanzaTreasures</p>
    </section>

    <footer>
        <p>© 2025 Esperanza. Handmade in Mexico.</p>
    </footer>

    <script>
        document.querySelectorAll('.nav-links a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        const cards = document.querySelectorAll('.product-card');
        const observer = new IntersectionObserver(entries => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'scale(1)';
                }
            });
        }, { threshold: 0.2 });

        cards.forEach(card => {
            card.style.opacity = '0';
            card.style.transform = 'scale(0.95)';
            card.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
            observer.observe(card);
        });
    </script>
</body>
</html>

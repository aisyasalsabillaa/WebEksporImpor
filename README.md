# WebEksporImpor
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PT Nusantara Global Trade - Impor Ekspor Terpercaya</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-color: #025c5b;
            --primary-dark: #014a49;
            --secondary-color: #1f5f99;
            --accent-color: #f8f9fa;
            --text-color: #2c3e50;
            --text-light: #7f8c8d;
            --white: #ffffff;
            --success-color: #27ae60;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--accent-color);
            overflow-x: hidden;
            padding-top: 80px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            width: 100%;
            box-sizing: border-box;
            overflow-x: hidden;
        }

        /* Header Styles */
        header {
            background: linear-gradient(135deg, var(--text-color) 0%, #34495e 100%);
            color: var(--white);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--white);
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
            flex-wrap: wrap;
        }

        .nav-menu a {
            color: var(--white);
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: all 0.3s ease;
        }

        .nav-menu a:hover {
            background-color: var(--primary-color);
            transform: translateY(-2px);
        }

        .mobile-menu-toggle {
            display: none;
            background: none;
            border: none;
            color: var(--white);
            font-size: 1.5rem;
            cursor: pointer;
            padding: 0.5rem;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--primary-dark) 100%);
            color: var(--white);
            padding: 150px 0 100px;
            text-align: center;
            position: relative;
            box-sizing: border-box;
            width: 100vw;
            max-width: 100%;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
        }

        .cta-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 15px 30px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-size: 1.1rem;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s ease;
            display: inline-block;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .btn-primary {
            background: linear-gradient(45deg, var(--primary-color), var(--primary-dark));
            color: var(--white);
        }

        .btn-secondary {
            background: transparent;
            color: var(--white);
            border: 2px solid var(--white);
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        /* Section Styles */
        .section {
            padding: 80px 0;
            width: 100%;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: var(--text-color);
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 80px;
            height: 4px;
            background: linear-gradient(45deg, var(--primary-color), var(--primary-dark));
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        /* Category Cards */
        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 3rem;
            margin-top: 4rem;
        }

        .category-card {
            background: var(--white);
            border-radius: 20px;
            padding: 3rem;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            border: 1px solid #f0f0f0;
        }

        .category-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 30px 60px rgba(0,0,0,0.15);
        }

        .category-header {
            text-align: center;
            margin-bottom: 2rem;
        }

        .category-icon {
            width: 80px;
            height: 80px;
            margin: 0 auto 1rem;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            color: var(--white);
        }

        .import-icon {
            background: linear-gradient(45deg, var(--primary-color), var(--primary-dark));
        }

        .export-icon {
            background: linear-gradient(45deg, var(--primary-color), var(--primary-dark));
        }

        .category-title {
            font-size: 2rem;
            color: var(--text-color);
            margin-bottom: 1rem;
        }

        .category-subtitle {
            color: var(--text-light);
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        /* Product Grid */
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .product-item {
            background: var(--accent-color);
            border-radius: 15px;
            padding: 1.5rem;
            text-align: center;
            transition: all 0.3s ease;
            border: 2px solid transparent;
        }

        .product-item:hover {
            background: var(--white);
            border-color: var(--primary-color);
            transform: translateY(-5px);
        }

        .product-icon {
            width: 60px;
            height: 60px;
            margin: 0 auto 1rem;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: var(--white);
            background: linear-gradient(45deg, var(--primary-color), var(--primary-dark));
        }

        .product-name {
            font-weight: 600;
            color: var(--text-color);
            margin-bottom: 0.5rem;
        }

        .product-desc {
            font-size: 0.9rem;
            color: var(--text-light);
            margin-bottom: 1rem;
        }

        .product-features {
            list-style: none;
            text-align: left;
        }

        .product-features li {
            padding: 0.3rem 0;
            color: #555;
            font-size: 0.85rem;
            position: relative;
            padding-left: 1.5rem;
        }

        .product-features li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--primary-color);
            font-weight: bold;
        }

        /* Features Section */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature-item {
            background: var(--white);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .feature-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .feature-icon {
            width: 70px;
            height: 70px;
            margin: 0 auto 1rem;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            color: var(--white);
            background: linear-gradient(45deg, var(--secondary-color), #0f4c75);
        }

        .feature-title {
            font-size: 1.3rem;
            color: var(--text-color);
            margin-bottom: 1rem;
        }

        .feature-desc {
            color: var(--text-light);
            line-height: 1.6;
        }

        /* Contact Section */
        .contact {
            background: linear-gradient(135deg, var(--text-color) 0%, #34495e 100%);
            color: var(--white);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
            gap: 3rem;
            align-items: start;
        }

        .contact-info {
            padding: 2rem;
        }

        .contact-items-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            gap: 1rem;
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: var(--primary-color);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--white);
            flex-shrink: 0;
            margin: 0;
        }

        .contact-form {
            background: rgba(255,255,255,0.1);
            padding: 2rem;
            border-radius: 15px;
            backdrop-filter: blur(10px);
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1rem;
            margin-bottom: 1rem;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--white);
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 10px;
            background: rgba(255,255,255,0.9);
            font-size: 1rem;
            font-family: inherit;
        }

        .form-group textarea {
            height: 120px;
            resize: vertical;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(2, 92, 91, 0.3);
        }

        /* Footer */
        footer {
            background: var(--text-color);
            color: var(--white);
            padding: 3rem 0 1rem;
            text-align: center;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
            text-align: left;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
            color: var(--primary-color);
        }

        .footer-section ul {
            list-style: none;
        }

        .footer-section ul li {
            padding: 0.3rem 0;
        }

        .footer-section ul li a {
            color: #bdc3c7;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-section ul li a:hover {
            color: var(--primary-color);
        }

        .footer-bottom {
            border-top: 1px solid #34495e;
            padding-top: 1rem;
            color: #95a5a6;
            text-align: center;
        }

        /* Scroll to top button */
        .scroll-to-top {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 50px;
            height: 50px;
            background: var(--primary-color);
            color: var(--white);
            border: none;
            border-radius: 50%;
            cursor: pointer;
            display: none;
            z-index: 1000;
            transition: all 0.3s ease;
            font-size: 1.2rem;
        }

        .scroll-to-top:hover {
            background: var(--primary-dark);
            transform: scale(1.1);
        }

        /* Responsive Design */
        @media (max-width: 1024px) {
            .category-grid {
                grid-template-columns: 1fr;
            }
            .contact-grid {
                grid-template-columns: 1fr;
            }
            .hero {
                padding: 120px 0 60px;
            }
            .hero h1 {
                font-size: 2.8rem;
            }
            .hero p {
                font-size: 1.1rem;
            }
        }

        @media (max-width: 768px) {
            .mobile-menu-toggle {
                display: block;
            }
            .nav-menu {
                display: none;
                flex-direction: column;
                width: 100%;
                position: absolute;
                top: 100%;
                left: 0;
                background: linear-gradient(135deg, var(--text-color) 0%, #34495e 100%);
                padding: 1rem 0;
            }
            .nav-menu.active {
                display: flex;
            }
            .nav-menu a {
                padding: 1rem;
                width: 100%;
                text-align: center;
            }
            .hero {
                padding: 90px 0 40px;
            }
            .hero h1 {
                font-size: 2.2rem;
            }
            .hero p {
                font-size: 1rem;
            }
            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }
            .category-card {
                padding: 1.5rem;
            }
            .form-row,
            .product-grid,
            .category-grid,
            .features-grid,
            .contact-grid {
                grid-template-columns: 1fr !important;
            }
            .contact-items-grid {
                grid-template-columns: 1fr !important;
                gap: 1.5rem;
            }
            .logo {
                font-size: 1.5rem;
            }
            .container {
                padding: 0 15px;
            }
            .section-title {
                font-size: 2rem;
            }
        }

        @media (max-width: 480px) {
            .hero {
                padding: 60px 0 30px;
            }
            .hero h1 {
                font-size: 1.8rem;
            }
            .hero p {
                font-size: 0.9rem;
            }
            .section {
                padding: 40px 0;
            }
            .category-card,
            .contact-form {
                padding: 1rem;
            }
            .section-title {
                font-size: 1.5rem;
            }
            .logo {
                font-size: 1.2rem;
            }
            .product-item {
                padding: 1rem;
            }
            .feature-item {
                padding: 1.5rem;
            }
            .contact-items-grid {
                gap: 1rem;
            }
            .btn {
                padding: 10px 20px;
                font-size: 1rem;
            }
        }

        /* Smooth scrolling */
        html {
            scroll-behavior: smooth;
        }

        /* Loading animation */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            animation: fadeInUp 0.6s ease forwards;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <div class="logo">🌍 PT Nusantara Global</div>
            <button class="mobile-menu-toggle" aria-label="Toggle menu" onclick="toggleMenu()">☰</button>
            <ul class="nav-menu">
                <li><a href="#home">Beranda</a></li>
                <li><a href="#impor">Import</a></li>
                <li><a href="#ekspor">Export</a></li>
                <li><a href="#layanan">Layanan</a></li>
                <li><a href="#kontak">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <h1 class="fade-in">Solusi Import-Export Terpercaya</h1>
            <p class="fade-in">Menghubungkan Indonesia dengan pasar global melalui perdagangan berkualitas tinggi</p>
            <div class="cta-buttons fade-in">
                <a href="#impor" class="btn btn-primary">Produk Import</a>
                <a href="#ekspor" class="btn btn-secondary">Produk Export</a>
            </div>
        </div>
    </section>

    <!-- Categories Section -->
    <section id="categories" class="section">
        <div class="container">
            <h2 class="section-title">Kategori Produk Kami</h2>
            
            <div class="category-grid">
                <!-- Impor Category -->
                <div id="impor" class="category-card">
                    <div class="category-header">
                        <div class="category-icon import-icon">📥</div>
                        <h3 class="category-title">IMPORT</h3>
                        <p class="category-subtitle">Menghadirkan produk berkualitas dari Afrika dan Ghana</p>
                    </div>
                    
                    <div class="product-grid">
                        <div class="product-item">
                            <div class="product-icon">🥥</div>
                            <h4 class="product-name">Shea Butter Afrika</h4>
                            <p class="product-desc">Mentega shea premium langsung dari Afrika</p>
                            <ul class="product-features">
                                <li>100% murni dan organik</li>
                                <li>Kualitas grade A</li>
                                <li>Sertifikat halal</li>
                                <li>Kemasan higienis</li>
                                <li>Harga kompetitif</li>
                            </ul>
                        </div>
                        
                        <div class="product-item">
                            <div class="product-icon">🌰</div>
                            <h4 class="product-name">Shea Butter Ghana</h4>
                            <p class="product-desc">Shea butter berkualitas premium dari Ghana</p>
                            <ul class="product-features">
                                <li>Tekstur halus dan lembut</li>
                                <li>Aroma natural</li>
                                <li>Kaya vitamin A, E, F</li>
                                <li>Anti-inflamasi alami</li>
                                <li>Cocok untuk kosmetik</li>
                            </ul>
                        </div>
                    </div>
                </div>

                <!-- Ekspor Category -->
                <div id="ekspor" class="category-card">
                    <div class="category-header">
                        <div class="category-icon export-icon">📤</div>
                        <h3 class="category-title">EXPORT</h3>
                        <p class="category-subtitle">Produk unggulan Indonesia untuk pasar internasional</p>
                    </div>
                    
                    <div class="product-grid">
                        <div class="product-item">
                            <div class="product-icon">🥥</div>
                            <h4 class="product-name">Kelapa Parut Kering</h4>
                            <p class="product-desc">Desiccated coconut berkualitas ekspor</p>
                            <ul class="product-features">
                                <li>Kadar air rendah (3%)</li>
                                <li>Warna putih bersih</li>
                                <li>Tekstur halus/medium/kasar</li>
                                <li>Kemasan vakum</li>
                                <li>Shelf life 12 bulan</li>
                            </ul>
                        </div>
                        
                        <div class="product-item">
                            <div class="product-icon">🍪</div>
                            <h4 class="product-name">Briket Kelapa</h4>
                            <p class="product-desc">Briket premium dari tempurung kelapa</p>
                            <ul class="product-features">
                                <li>Kalor tinggi 7000+ kcal/kg</li>
                                <li>Low ash content (2-4%)</li>
                                <li>Burn time 3-4 jam</li>
                                <li>Smokeless & odorless</li>
                                <li>Eco-friendly</li>
                            </ul>
                        </div>
                        
                        <div class="product-item">
                            <div class="product-icon">🧅</div>
                            <h4 class="product-name">Bawang Goreng</h4>
                            <p class="product-desc">Fried shallot crispy kualitas premium</p>
                            <ul class="product-features">
                                <li>Bawang merah pilihan</li>
                                <li>Tekstur crispy tahan lama</li>
                                <li>Tanpa pengawet buatan</li>
                                <li>Kemasan kedap udara</li>
                                <li>Siap pakai dan tahan lama</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="layanan" class="section" style="background: white;">
        <div class="container">
            <h2 class="section-title">Layanan Unggulan Kami</h2>
            
            <div class="features-grid">
                <div class="feature-item">
                    <div class="feature-icon">🚢</div>
                    <h3 class="feature-title">Logistik & Pengiriman</h3>
                    <p class="feature-desc">Sistem logistik terintegrasi dengan tracking real-time untuk memastikan produk sampai tepat waktu dan dalam kondisi prima.</p>
                </div>
                
                <div class="feature-item">
                    <div class="feature-icon">📋</div>
                    <h3 class="feature-title">Sertifikasi & Dokumen</h3>
                    <p class="feature-desc">Pengurusan lengkap dokumen import-export, sertifikat halal, BPOM, dan perizinan lainnya sesuai regulasi internasional.</p>
                </div>
                
                <div class="feature-item">
                    <div class="feature-icon">🔍</div>
                    <h3 class="feature-title">Quality Control</h3>
                    <p class="feature-desc">Sistem kontrol kualitas ketat mulai dari seleksi supplier hingga inspeksi final sebelum pengiriman ke konsumen.</p>
                </div>
                
                <div class="feature-item">
                    <div class="feature-icon">💰</div>
                    <h3 class="feature-title">Harga Kompetitif</h3>
                    <p class="feature-desc">Harga terbaik di pasar dengan sistem pembayaran fleksibel dan transparansi penuh dalam setiap transaksi.</p>
                </div>
                
                <div class="feature-item">
                    <div class="feature-icon">🤝</div>
                    <h3 class="feature-title">Kemitraan Jangka Panjang</h3>
                    <p class="feature-desc">Membangun hubungan bisnis jangka panjang dengan komitmen pada kepuasan pelanggan dan pertumbuhan bersama.</p>
                </div>
                
                <div class="feature-item">
                    <div class="feature-icon">🌐</div>
                    <h3 class="feature-title">Jaringan Global</h3>
                    <p class="feature-desc">Jaringan supplier dan distributor internasional yang luas untuk memenuhi kebutuhan pasar domestik dan ekspor.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="kontak" class="section contact">
        <div class="container">
            <h2 class="section-title" style="color: white;">Hubungi Kami</h2>
            
            <div class="contact-grid">
                <div class="contact-info">
                    <h3 style="margin-bottom: 2rem;">Informasi Kontak</h3>
                    
                    <div class="contact-items-grid">
                        <div class="contact-item">
                            <div class="contact-icon">📍</div>
                            <div>
                                <h4>Alamat Kantor</h4>
                                <p>Jl. Perdagangan Internasional No. 123<br>Surabaya, Jawa Timur 60115<br>Indonesia</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">📞</div>
                            <div>
                                <h4>Telepon & WhatsApp</h4>
                                <p>+62 31 1234 5678<br>+62 812 3456 7890</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">✉</div>
                            <div>
                                <h4>Email</h4>
                                <p>info@nusantaraglobal.co.id<br>export@nusantaraglobal.co.id</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">⏰</div>
                            <div>
                                <h4>Jam Operasional</h4>
                                <p>Senin - Jumat: 08:00 - 17:00<br>Sabtu: 08:00 - 14:00</p>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Add contact form here if needed -->
            </div>
        </div>
    </section>

    <button class="scroll-to-top" onclick="scrollToTop()">⬆</button>

    <script>
        function toggleMenu() {
            const navMenu = document.querySelector('.nav-menu');
            navMenu.classList.toggle('active');
        }

        function scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        window.addEventListener('scroll', () => {
            const scrollToTopBtn = document.querySelector('.scroll-to-top');
            if (window.scrollY > 300) {
                scrollToTopBtn.style.display = 'block';
            } else {
                scrollToTopBtn.style.display = 'none';
            }
        });

        // Add fade-in effect to sections on scroll
        const sections = document.querySelectorAll('.section, .hero');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('fade-in');
                }
            });
        }, { threshold: 0.1 });

        sections.forEach(section => {
            observer.observe(section);
        });
    </script>
</body>
</html>

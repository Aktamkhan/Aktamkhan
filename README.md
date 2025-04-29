<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Boshquduq Mahalla Portali</title>

    <style>
        /* Umumiy sozlamalar */
        body {
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background-color: #e6f2ff; /* Ochiq ko‘k fon */
            color: #003366; /* Qoramtir ko‘k matn */
        }

        /* Header */
        header {
            background-color: #003366; /* Chuqur ko‘k */
            color: white;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        header .logo h1 {
            margin: 0;
            font-size: 24px;
        }

        header .top-menu a {
            color: #99ccff; /* Ochiq ko‘k link */
            text-decoration: none;
            margin-left: 15px;
        }

        header .top-menu a:hover {
            color: white;
        }

        /* Main Navigation */
        .main-nav {
            background: #0059b3; /* O‘rtacha ko‘k */
            padding: 0.5rem 0;
        }

        .main-nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            margin: 0;
            padding: 0;
        }

        .main-nav ul li {
            margin: 0 20px;
        }

        .main-nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
        }

        .main-nav ul li a:hover {
            color: #cce6ff; /* Ochiqroq ko‘k */
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 3rem 1rem;
            background: linear-gradient(rgba(0,51,102,0.7), rgba(0,51,102,0.7)), url('hero-image.jpg') no-repeat center center/cover;
            color: white;
        }

        .hero h2 {
            font-size: 32px;
            margin-bottom: 1rem;
        }

        /* Sections */
        .news, .services, .about, .contact {
            padding: 2rem;
            background: white;
            margin: 1rem;
            border-radius: 8px;
        }

        .news-cards, .services-cards {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            margin-top: 1rem;
        }

        .card, .service-card {
            background: #cce6ff; /* Ochiq ko‘k kartalar */
            padding: 1rem;
            border-radius: 8px;
            flex: 1 1 30%;
            min-width: 250px;
            text-align: center;
        }

        /* Contact form */
        form {
            display: flex;
            flex-direction: column;
        }

        form input, form textarea {
            padding: 10px;
            margin-bottom: 1rem;
            border: 1px solid #99ccff;
            border-radius: 5px;
        }

        form button {
            padding: 10px;
            background: #0059b3;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        form button:hover {
            background: #003366;
        }

        /* Footer */
        footer {
            background: #003366;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }

        footer .social-links a {
            color: #white;
            margin: 0 10px;
            text-decoration: none;
        }

        footer .social-links a:hover {
            text-decoration: underline;
        }

        /* Responsive dizayn */
        @media (max-width: 768px) {
            .news-cards, .services-cards {
                flex-direction: column;
            }
        }
    </style>

</head>

<body>

    <!-- Header -->
    <header>
        <div class="logo">
            <h1>Boshquduq.uz</h1>
        </div>
        <nav class="top-menu">
            <a href="#">Kirish</a>
            <a href="#">Ro'yxatdan o'tish</a>
        </nav>
    </header>

    <!-- Main Navigation -->
    <nav class="main-nav">
        <ul>
            <li><a href="#">Bosh sahifa</a></li>
            <li><a href="#">Yangiliklar</a></li>
            <li><a href="#">Tadbirlar</a></li>
            <li><a href="#">Xizmatlar</a></li>
            <li><a href="#">Aloqa</a></li>
        </ul>
    </nav>

    <!-- Hero Section -->
    <section class="hero">
        <h2>Mahallamiz — Yagona va Hamjihat Oila</h2>
        <img src="hero-image.jpg" alt="Mahalla rasmi" style="max-width:100%; height:auto; margin-top:20px;">
    </section>

    <!-- News Section -->
    <section class="news">
        <h2>So‘nggi Yangiliklar</h2>
        <div class="news-cards">
            <div class="card">
                <h3>Hashar kuni belgilandi</h3>
                <p>28-aprel, soat 8:00 da umumiy hashar bo‘lib o‘tadi.</p>
            </div>
            <div class="card">
                <h3>Chiqindi yig'ish haftaligi</h3>
                <p>Har bir ko'cha o'z hududini tozalash ishlariga qatnashadi.</p>
            </div>
            <div class="card">
                <h3>Yoshlar sport musobaqasi</h3>
                <p>8-may kuni stadionda katta sport tadbiri bo‘lib o‘tadi!</p>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services">
        <h2>Xizmatlar</h2>
        <div class="services-cards">
            <div class="service-card">Murojaat yuborish</div>
            <div class="service-card">Elektron ariza topshirish</div>
            <div class="service-card">Fikr-mulohaza bildirish</div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about">
        <h2>Mahalla haqida</h2>
        <p>Bizning mahalla uzoq tarixga ega bo‘lib, oqsoqollarimiz va yoshlarimiz bilan faxrlanamiz. Mahalla hamjihatligi va madaniyati har birimizni birlashtiradi.</p>
    </section>

    <!-- Contact Section -->
    <section class="contact">
        <h2>Aloqa</h2>
        <form>
            <input type="text" placeholder="Ismingiz" required>
            <input type="tel" placeholder="Telefon raqamingiz" required>
            <textarea placeholder="Xabaringiz" rows="5" required></textarea>
            <button type="submit">Yuborish</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 AkSoftUz</p>
        <div class="social-links">
            <a href="#">Facebook</a> |
            <a href="#">Instagram</a> |
            <a href="#">Telegram</a> |
            <a href="#">Email</a>
        </div>
    </footer>

</body>
</html>
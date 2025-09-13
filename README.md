<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nurul Falah Preschool - Islamic Education Centre</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary-blue: #0056b3;
            --primary-orange: #ff8c00;
            --primary-brown: #8b4513;
            --light-blue: #e6f2ff;
            --light-orange: #fff0e6;
            --light-brown: #f5f0e8;
            --dark-blue: #003366;
        }

        body {
            background-color: #f9f7f3;
            color: #333;
            line-height: 1.6;
        }

        /* Header Styles */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 5%;
            max-width: 1400px;
            margin: 0 auto;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo img {
            height: 70px;
            margin-right: 15px;
        }

        .logo-text {
            display: flex;
            flex-direction: column;
        }

        .logo-text h1 {
            color: var(--primary-orange);
            font-size: 28px;
            font-weight: bold;
            margin-bottom: 5px;
        }

        .logo-text p {
            color: var(--dark-blue);
            font-size: 14px;
            font-weight: 500;
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 25px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--dark-blue);
            font-weight: 600;
            font-size: 16px;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--primary-orange);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 51, 102, 0.7), rgba(0, 51, 102, 0.7)), url('https://z-cdn-media.chatglm.cn/files/6ed921d3-f679-4fac-9a11-4aa40d66f534_Gambar%20Kegiatan5.jpg?auth_key=1789294101-f9b76a811f854df284d00366662a7436-0-a132e35859dbf38e16b7cf7e79b4c4c2');
            background-size: cover;
            background-position: center;
            height: 500px;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
        }

        .hero-content {
            max-width: 800px;
            padding: 0 20px;
        }

        .hero-content h2 {
            font-size: 48px;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        .hero-content p {
            font-size: 20px;
            margin-bottom: 30px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
        }

        .btn {
            display: inline-block;
            background-color: var(--primary-orange);
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: bold;
            font-size: 16px;
            transition: all 0.3s;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }

        .btn:hover {
            background-color: #e67e00;
            transform: translateY(-3px);
            box-shadow: 0 6px 8px rgba(0,0,0,0.15);
        }

        /* About Section */
        .about {
            padding: 80px 5%;
            background-color: white;
        }

        .section-container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            color: var(--dark-blue);
            font-size: 36px;
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }

        .section-title h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--primary-orange);
            border-radius: 2px;
        }

        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .about-text {
            flex: 1;
        }

        .about-text h3 {
            color: var(--primary-orange);
            font-size: 28px;
            margin-bottom: 20px;
        }

        .about-text p {
            margin-bottom: 20px;
            font-size: 16px;
        }

        .about-image {
            flex: 1;
            text-align: center;
        }

        .about-image img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        /* Activities Section */
        .activities {
            padding: 80px 5%;
            background-color: var(--light-brown);
        }

        .activities-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .activity-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .activity-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }

        .activity-image {
            height: 200px;
            overflow: hidden;
        }

        .activity-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .activity-card:hover .activity-image img {
            transform: scale(1.1);
        }

        .activity-content {
            padding: 20px;
        }

        .activity-content h3 {
            color: var(--dark-blue);
            font-size: 22px;
            margin-bottom: 10px;
        }

        .activity-content p {
            color: #666;
            font-size: 15px;
        }

        /* Gallery Section */
        .gallery {
            padding: 80px 5%;
            background-color: white;
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 50px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 8px;
            height: 250px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }

        .gallery-item:hover img {
            transform: scale(1.1);
        }

        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0,0,0,0.7));
            color: white;
            padding: 15px;
            transform: translateY(100%);
            transition: transform 0.3s;
        }

        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }

        /* Testimonials Section */
        .testimonials {
            padding: 80px 5%;
            background-color: var(--light-blue);
        }

        .testimonial-container {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .testimonial {
            background-color: white;
            border-radius: 10px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .testimonial p {
            font-style: italic;
            margin-bottom: 20px;
            font-size: 16px;
        }

        .testimonial h4 {
            color: var(--primary-orange);
            font-weight: bold;
        }

        /* Contact Section */
        .contact {
            padding: 80px 5%;
            background-color: white;
        }

        .contact-container {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            gap: 50px;
        }

        .contact-info {
            flex: 1;
        }

        .contact-info h3 {
            color: var(--dark-blue);
            font-size: 28px;
            margin-bottom: 20px;
        }

        .contact-info p {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }

        .contact-info i {
            color: var(--primary-orange);
            margin-right: 15px;
            font-size: 20px;
            width: 25px;
        }

        .contact-form {
            flex: 1;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }

        .form-group textarea {
            height: 150px;
            resize: vertical;
        }

        /* Footer */
        footer {
            background-color: var(--dark-blue);
            color: white;
            padding: 50px 5%;
            text-align: center;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
        }

        .footer-logo {
            flex: 1;
            min-width: 300px;
            margin-bottom: 30px;
        }

        .footer-logo img {
            height: 60px;
            margin-bottom: 15px;
        }

        .footer-links {
            flex: 1;
            min-width: 300px;
            margin-bottom: 30px;
        }

        .footer-links h3 {
            margin-bottom: 20px;
            font-size: 20px;
        }

        .footer-links ul {
            list-style: none;
        }

        .footer-links ul li {
            margin-bottom: 10px;
        }

        .footer-links ul li a {
            color: #ccc;
            text-decoration: none;
            transition: color 0.3s;
        }

        .footer-links ul li a:hover {
            color: white;
        }

        .footer-social {
            flex: 1;
            min-width: 300px;
            margin-bottom: 30px;
        }

        .footer-social h3 {
            margin-bottom: 20px;
            font-size: 20px;
        }

        .social-icons {
            display: flex;
            justify-content: center;
            gap: 15px;
        }

        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            color: white;
            font-size: 18px;
            transition: background-color 0.3s;
        }

        .social-icons a:hover {
            background-color: var(--primary-orange);
        }

        .copyright {
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 14px;
            color: #ccc;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .about-content {
                flex-direction: column;
            }
            
            .contact-container {
                flex-direction: column;
            }
        }

        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                padding: 15px;
            }
            
            .logo {
                margin-bottom: 15px;
            }
            
            nav ul {
                flex-wrap: wrap;
                justify-content: center;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            .hero-content h2 {
                font-size: 36px;
            }
            
            .hero-content p {
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="header-container">
            <div class="logo">
                <img src="https://z-cdn-media.chatglm.cn/files/3a55aeff-b9c5-424e-96c0-890cdaf1deb2_Gambar%20RA%20NURUL%20FALAH.jpg?auth_key=1789294101-8fef3037666c4bf7b8c459401a17c350-0-b34513c9a827a210a3929643ee70e85c" alt="Nurul Falah Logo">
                <div class="logo-text">
                    <h1>Nurul Falah</h1>
                    <p>Pusat Pendidikan Islam Prasekolah</p>
                </div>
            </div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#activities">Activities</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <h2>Selamat datang di PAUD Nurul Falah</h2>
            <p> Membina generasi muda dengan nilai-nilai Islam dan pendidikan yang berkualitas</p>
            <a href="#about" class="btn">Pelajari Lebih Lanjut</a>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="section-container">
            <div class="section-title">
                <h2>Tentang Sekolah Kami</h2>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>Pendidikan Islam dengan Pendekatan Modern</h3>
                    <p>Prasekolah Nurul Falah adalah pusat pendidikan Islam terkemuka yang berdedikasi untuk menyediakan lingkungan yang mendukung bagi para pelajar muda. Kami memadukan nilai-nilai Islam tradisional dengan metodologi pengajaran modern untuk menciptakan pengalaman belajar yang holistik.</p>
                    <p>Kurikulum kami dirancang untuk menumbuhkan perkembangan intelektual, spiritual, emosional, dan fisik anak usia 3-6 tahun. Kami berfokus pada pembentukan fondasi yang kuat dalam ajaran Islam sekaligus mempersiapkan anak-anak untuk kesuksesan akademis di masa depan.</p>
                    <a href="#contact" class="btn">Hubungi kami</a>
                </div>
                <div class="about-image">
                    <img src="https://z-cdn-media.chatglm.cn/files/e17d94a6-28fb-4b2d-99fb-9638f7616b32_Gambar%20Kegiatan4.jpg?auth_key=1789294101-25ded6cc7d7447d8ae2cb4d5aa71f515-0-16ebb825f66e09ee0c40e7b181d743fa" alt="Classroom Activity">
                </div>
            </div>
        </div>
    </section>

    <!-- Activities Section -->
    <section class="activities" id="activities">
        <div class="section-container">
            <div class="section-title">
                <h2>Aktivitas Kami</h2>
            </div>
            <div class="activities-grid">
                <div class="activity-card">
                    <div class="activity-image">
                        <img src="https://z-cdn-media.chatglm.cn/files/6ed921d3-f679-4fac-9a11-4aa40d66f534_Gambar%20Kegiatan5.jpg?auth_key=1789294101-f9b76a811f854df284d00366662a7436-0-a132e35859dbf38e16b7cf7e79b4c4c2" alt="Ramadhan Show">
                    </div>
                    <div class="activity-content">
                        <h3>Ramadhan Show</h3>
                        <p>Pertunjukan dan kegiatan khusus selama bulan suci Ramadan untuk mengajarkan anak-anak tentang tradisi Islam.</p>
                    </div>
                </div>
                <div class="activity-card">
                    <div class="activity-image">
                        <img src="https://z-cdn-media.chatglm.cn/files/df38371a-9d11-42c2-97dc-e3f60233235f_Gambar%20Kegiatan1.jpg?auth_key=1789294101-2d97d8e7c7df43aeb3be93c880b6cef6-0-28086c24fa410b6225698e4dbf237294" alt="Creative Activities">
                    </div>
                    <div class="activity-content">
                        <h3>Kegiatan Kreatif</h3>
                        <p>Sesi seni dan kerajinan yang mendorong kreativitas dan ekspresi diri pada pelajar muda.</p>
                    </div>
                </div>
                <div class="activity-card">
                    <div class="activity-image">
                        <img src="https://z-cdn-media.chatglm.cn/files/ad316a97-d673-4ccc-af43-4bab3b4c0775_Gambar%20Kegiatan6.jpg?auth_key=1789294101-cbd32d87c32149018dd8d5feec85a0ed-0-8bdbae163dd64380610b5f02ba3c36ed" alt="Cooking Class">
                    </div>
                    <div class="activity-content">
                        <h3>Kelas Memasak</h3>
                        <p>Sesi memasak yang menyenangkan dan mendidik yang mengajarkan anak-anak tentang nutrisi dan keterampilan memasak dasar.</p>
                    </div>
                </div>
                <div class="activity-card">
                    <div class="activity-image">
                        <img src="https://z-cdn-media.chatglm.cn/files/eab549f7-7e2b-45ab-8eb9-35b8c0c7db0a_Gambar%20Kegiatan2.jpg?auth_key=1789294101-3baa910d3d424133ad753f5bbf0d7eb1-0-c55735636ace82fbd4b820909ac5b53" alt="Rumah Tahfidz">
                    </div>
                    <div class="activity-content">
                        <h3>Rumah Tahfidz</h3>
                        <p>Program menghafal Al-Quran yang dirancang khusus untuk anak-anak muda untuk membangun fondasi yang kuat dalam pendidikan Islam.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section class="gallery" id="gallery">
        <div class="section-container">
            <div class="section-title">
                <h2>Galeri Sekolah</h2>
            </div>
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/1de6d634-6a5b-4c1b-ba68-16fc3b381ff4_Gambar%20Kegiatan3.jpg?auth_key=1789294101-fd6ea06706974aee92819fe5ae4c01de-0-338f0dac5ba32978ff44634251d14ce4" alt="Class B Activity">
                    <div class="gallery-overlay">
                        <p>Class B Activities</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/5ee1b89c-84e8-4a88-81a8-7bb83cc9d7ad_Gambar%20Kegiatan7.jpg?auth_key=1789294101-aee10226e7a842ec8ef15ec9ab271c62-0-3b6ae236f9cd98da8bdc39a74f2b3ca" alt="Creative Theme">
                    <div class="gallery-overlay">
                        <p>Creative Theme Day</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/e17d94a6-28fb-4b2d-99fb-9638f7616b32_Gambar%20Kegiatan4.jpg?auth_key=1789294101-25ded6cc7d7447d8ae2cb4d5aa71f515-0-16ebb825f66e09ee0c40e7b181d743fa" alt="Class A Activity">
                    <div class="gallery-overlay">
                        <p>Class A Activities</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/df38371a-9d11-42c2-97dc-e3f60233235f_Gambar%20Kegiatan1.jpg?auth_key=1789294101-2d97d8e7c7df43aeb3be93c880b6cef6-0-28086c24fa410b6225698e4dbf237294" alt="Creative Activities">
                    <div class="gallery-overlay">
                        <p>Creative Activities</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/ad316a97-d673-4ccc-af43-4bab3b4c0775_Gambar%20Kegiatan6.jpg?auth_key=1789294101-cbd32d87c32149018dd8d5feec85a0ed-0-8bdbae163dd64380610b5f02ba3c36ed" alt="Cooking Class">
                    <div class="gallery-overlay">
                        <p>Cooking Class</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/eab549f7-7e2b-45ab-8eb9-35b8c0c7db0a_Gambar%20Kegiatan2.jpg?auth_key=1789294101-3baa910d3d424133ad753f5bbf0d7eb1-0-c55735636ace82fbd4b820909ac5b53" alt="Rumah Tahfidz">
                    <div class="gallery-overlay">
                        <p>Rumah Tahfidz</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/6ed921d3-f679-4fac-9a11-4aa40d66f534_Gambar%20Kegiatan5.jpg?auth_key=1789294101-f9b76a811f854df284d00366662a7436-0-a132e35859dbf38e16b7cf7e79b4c4c2" alt="Ramadhan Show">
                    <div class="gallery-overlay">
                        <p>Ramadhan Show</p>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://z-cdn-media.chatglm.cn/files/3a55aeff-b9c5-424e-96c0-890cdaf1deb2_Gambar%20RA%20NURUL%20FALAH.jpg?auth_key=1789294101-8fef3037666c4bf7b8c459401a17c350-0-b34513c9a827a210a3929643ee70e85c" alt="School Logo">
                    <div class="gallery-overlay">
                        <p>Nurul Falah Preschool</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials">
        <div class="section-container">
            <div class="section-title">
                <h2>Apa Kata Orang Tua</h2>
            </div>
            <div class="testimonial-container">
                <div class="testimonial">
                    <p>"Prasekolah Nurul Falah telah memberikan fondasi yang sangat baik bagi anak saya. Nilai-nilai Islam yang dipadukan dengan metode pengajaran modern telah membantu anak saya tumbuh secara akademis dan spiritual."</p>
                    <h4>- Fatima Ahmad, Parent</h4>
                </div>
                <div class="testimonial">
                    <p>"Para guru di Nurul Falah sangat peduli dan berdedikasi. Anak saya senang bersekolah setiap hari dan telah mengembangkan kecintaan terhadap pembelajaran dan praktik-praktik Islam."</p>
                    <h4>- Ahmad Hassan, Parent</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="section-container">
            <div class="section-title">
                <h2>Hubungi kami</h2>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Hubungi Kami</h3>
                    <p><i class="fas fa-map-marker-alt"></i> Jln. Bbk. Tarogong Gg.Laksana I no. 22 Rt.02 Rw.05 kel. Bbk. Tarogong Kec. Bojongloa Kaler Kota bandung
</p>
                    <p><i class="fas fa-phone"></i> 089514120898</p>
                    <p><i class="fas fa-envelope"></i> nurulfalahpreschool94@gmail.com</p>
                    <p><i class="fas fa-clock"></i> Senin - Jumat: 07.30 - 15.30</p>
                    <p><i class="fas fa-clock"></i> Sabtu: 08.00 - 12.00</p>
                </div>
                <div class="contact-form">
                    <form>
                        <div class="form-group">
                            <input type="text" placeholder="Your Name" required>
                        </div>
                        <div class="form-group">
                            <input type="email" placeholder="Your Email" required>
                        </div>
                        <div class="form-group">
                            <input type="text" placeholder="Subject" required>
                        </div>
                        <div class="form-group">
                            <textarea placeholder="Your Message" required></textarea>
                        </div>
                        <button type="submit" class="btn">Kirim Pesan</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-content">
            <div class="footer-logo">
                <img src="https://z-cdn-media.chatglm.cn/files/3a55aeff-b9c5-424e-96c0-890cdaf1deb2_Gambar%20RA%20NURUL%20FALAH.jpg?auth_key=1789294101-8fef3037666c4bf7b8c459401a17c350-0-b34513c9a827a210a3929643ee70e85c" alt="Nurul Falah Logo">
                <p>Pusat Pendidikan Islam PAUD Nurul Falah</p>
                <p>Membina generasi muda dengan nilai-nilai Islam dan pendidikan yang berkualitas</p>
            </div>
            <div class="footer-links">
                <h3>Tautan Cepat</h3>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#activities">Activities</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
            <div class="footer-social">
                <h3>Follow Us</h3>
                <div class="social-icons">
                    <a href="#"><i class="fab fa-facebook-f"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-instagram"></i></a>
                    <a href="#"><i class="fab fa-youtube"></i></a>
                </div>
            </div>
        </div>
        <div class="copyright">
            <p>&copy; PAUD Nurul Falah 2023. Semua Hak Dilindungi Undang-undang.</p>
        </div>
    </footer>
</body>
</html>

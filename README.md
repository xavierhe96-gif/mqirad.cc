
<html lang="ms">
<head>
    <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>M-Qirad - Perundingan Kewangan Profesional</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #ffffff;
            color: #333333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Navigation */
        header {
            background-color: #ffffff;
            color: #1a472a;
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.08);
            border-bottom: 1px solid #eaeaea;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo-img {
            height: 70px;
            width: auto;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
        }
        
        .logo-text h1 {
            font-size: 1.8rem;
            margin-bottom: 5px;
            color: #1a472a;
        }
        
        .logo-text p {
            font-size: 0.9rem;
            color: #2d5e3f;
        }
        
        .contact-info {
            display: flex;
            align-items: center;
            gap: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.9rem;
        }
        
        .contact-icon {
            color: #2d5e3f;
            font-size: 1.2rem;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(255, 255, 255, 0.95), rgba(255, 255, 255, 0.95)), url('https://images.unsplash.com/photo-1554224155-6726b3ff858f?ixlib=rb-4.0.3&auto=format&fit=crop&w=1400&q=80');
            background-size: cover;
            background-position: center;
            color: #000000;
            padding: 80px 0;
            text-align: center;
            border-bottom: 1px solid #eaeaea;
        }
        
        .hero-content h2 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            color: #1a472a;
        }
        
        .hero-content p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 30px;
            color: #333333;
        }
        
        .highlight {
            background-color: #1a472a;
            color: #ffffff;
            padding: 15px 25px;
            border-radius: 8px;
            display: inline-block;
            font-weight: bold;
            font-size: 1.3rem;
            margin-top: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        /* Company Info */
        .company-info {
            padding: 60px 0;
            background-color: #fafafa;
            border-bottom: 1px solid #eaeaea;
        }
        
        .section-title {
            text-align: center;
            color: #1a472a;
            margin-bottom: 40px;
            font-size: 2rem;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 4px;
            background-color: #2d5e3f;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .company-details {
            background-color: #ffffff;
            padding: 30px;
            border-radius: 10px;
            margin-bottom: 30px;
            border-left: 5px solid #1a472a;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }
        
        .company-details h3 {
            color: #1a472a;
            margin-bottom: 15px;
            font-size: 1.5rem;
        }
        
        .company-details p {
            margin-bottom: 15px;
            color: #333333;
        }
        
        .age-groups {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 30px;
            flex-wrap: wrap;
        }
        
        .age-group {
            background-color: #ffffff;
            color: #000000;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            min-width: 200px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border: 2px solid #1a472a;
        }
        
        .age-group h4 {
            font-size: 1.8rem;
            margin-bottom: 10px;
            color: #1a472a;
        }
        
        /* Benefits Section */
        .benefits {
            padding: 60px 0;
            background-color: #ffffff;
            border-bottom: 1px solid #eaeaea;
        }
        
        .benefits-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .benefit-card {
            background-color: #fafafa;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
            border-top: 4px solid #1a472a;
            transition: transform 0.3s ease;
        }
        
        .benefit-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
        }
        
        .benefit-icon {
            font-size: 2.5rem;
            color: #1a472a;
            margin-bottom: 15px;
        }
        
        .benefit-card h3 {
            color: #1a472a;
            margin-bottom: 10px;
        }
        
        .benefit-card p {
            color: #333333;
        }
        
        /* Testimonials */
        .testimonials {
            padding: 60px 0;
            background-color: #fafafa;
            border-bottom: 1px solid #eaeaea;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .testimonial-card {
            background-color: #ffffff;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
            border-left: 4px solid #1a472a;
        }
        
        .customer-name {
            font-weight: bold;
            color: #1a472a;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .customer-name i {
            color: #2d5e3f;
        }
        
        .testimonial-card p {
            color: #333333;
        }
        
        /* NEW: WhatsApp Testimonials Section */
        .whatsapp-testimonials {
            padding: 60px 0;
            background-color: #ffffff;
            border-bottom: 1px solid #eaeaea;
        }
        
        .whatsapp-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .whatsapp-card {
            background-color: #fafafa;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.06);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid #e0e0e0;
        }
        
        .whatsapp-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 25px rgba(0, 0, 0, 0.1);
        }
        
        .whatsapp-header {
            background-color: #1a472a;
            color: white;
            padding: 15px 20px;
            display: flex;
            align-items: center;
            gap: 12px;
        }
        
        .whatsapp-icon {
            font-size: 1.5rem;
            color: #25D366;
        }
        
        .whatsapp-customer {
            font-weight: bold;
            font-size: 1.1rem;
        }
        
        .whatsapp-image-container {
            padding: 20px;
            background-color: white;
            text-align: center;
        }
        
        .whatsapp-image {
            max-width: 100%;
            height: auto;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.08);
            border: 1px solid #eaeaea;
            transition: transform 0.3s ease;
        }
        
        .whatsapp-image:hover {
            transform: scale(1.02);
        }
        
        .whatsapp-info {
            padding: 15px 20px;
            background-color: #f5f9f7;
            border-top: 1px solid #e0e0e0;
        }
        
        .whatsapp-amount {
            font-weight: bold;
            color: #1a472a;
            font-size: 1.2rem;
            margin-bottom: 8px;
        }
        
        .whatsapp-message {
            color: #333333;
            font-size: 0.95rem;
            font-style: italic;
            margin-bottom: 10px;
        }
        
        .whatsapp-date {
            color: #666;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        /* Application Form */
        .application {
            padding: 60px 0;
            background-color: #ffffff;
            border-bottom: 1px solid #eaeaea;
        }
        
        .form-container {
            background-color: #fafafa;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            max-width: 800px;
            margin: 0 auto;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: #1a472a;
            font-weight: 600;
        }
        
        .form-group input, .form-group select {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            background-color: #ffffff;
        }
        
        /* Enhanced Calendar Styling - Boleh Pilih Semua Tarikh */
        .calendar-container {
            position: relative;
        }
        
        .calendar-container input[type="date"] {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            background-color: #ffffff;
            cursor: pointer;
        }
        
        .calendar-container i {
            position: absolute;
            right: 15px;
            top: 50%;
            transform: translateY(-50%);
            color: #1a472a;
            pointer-events: none;
            z-index: 1;
        }
        
        /* Styling for date input in different browsers */
        input[type="date"] {
            -webkit-appearance: none;
            -moz-appearance: none;
            appearance: none;
            padding-right: 40px;
        }
        
        /* Custom styling for the calendar popup */
        input[type="date"]::-webkit-calendar-picker-indicator {
            background: transparent;
            bottom: 0;
            color: transparent;
            cursor: pointer;
            height: auto;
            left: 0;
            position: absolute;
            right: 0;
            top: 0;
            width: auto;
            opacity: 0;
        }
        
        .requirements {
            background-color: #ffffff;
            padding: 25px;
            border-radius: 10px;
            margin-top: 30px;
            border: 1px solid #e0e0e0;
        }
        
        .requirements h3 {
            color: #1a472a;
            margin-bottom: 15px;
        }
        
        .requirements ul {
            list-style-type: none;
            padding-left: 0;
        }
        
        .requirements li {
            margin-bottom: 10px;
            padding-left: 25px;
            position: relative;
            color: #333333;
        }
        
        .requirements li:before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #1a472a;
            font-weight: bold;
        }
        
        .submit-btn {
            background-color: #1a472a;
            color: #ffffff;
            border: none;
            padding: 15px 30px;
            font-size: 1.1rem;
            border-radius: 5px;
            cursor: pointer;
            display: block;
            width: 100%;
            margin-top: 20px;
            font-weight: bold;
            transition: all 0.3s ease;
        }
        
        .submit-btn:hover {
            background-color: #2d5e3f;
            box-shadow: 0 5px 15px rgba(26, 71, 42, 0.2);
        }
        
        /* WhatsApp Button */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.4);
            z-index: 1000;
            transition: all 0.3s ease;
            text-decoration: none;
        }
        
        .whatsapp-float:hover {
            background-color: #128C7E;
            transform: scale(1.1);
        }
        
        /* Google Maps Section */
        .location {
            padding: 60px 0;
            background-color: #fafafa;
            border-bottom: 1px solid #eaeaea;
        }
        
        .map-container {
            margin-top: 30px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            height: 450px;
        }
        
        .map-container iframe {
            width: 100%;
            height: 100%;
            border: none;
        }
        
        .location-info {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 10px;
            margin-top: 20px;
            border-left: 4px solid #1a472a;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.03);
        }
        
        .location-info h3 {
            color: #1a472a;
            margin-bottom: 10px;
            font-size: 1.3rem;
        }
        
        .location-info p {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
            color: #333333;
        }
        
        .location-info i {
            color: #1a472a;
            width: 20px;
        }
        
        /* Operating Hours */
        .operating-hours {
            padding: 40px 0;
            background-color: #ffffff;
            border-bottom: 1px solid #eaeaea;
        }
        
        .hours-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #fafafa;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.03);
        }
        
        .hours-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .hours-day {
            padding: 15px;
            border-radius: 8px;
            background-color: #ffffff;
            border: 1px solid #e0e0e0;
        }
        
        .hours-day.special {
            background-color: #f5f9f7;
            border-left: 4px solid #1a472a;
        }
        
        .hours-day.closed {
            background-color: #f9f5f5;
            border-left: 4px solid #a83232;
        }
        
        .day-name {
            font-weight: bold;
            color: #1a472a;
            margin-bottom: 5px;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .day-name i {
            color: #1a472a;
        }
        
        .day-time {
            color: #333333;
        }
        
        /* Footer */
        footer {
            background-color: #1a472a;
            color: #ffffff;
            padding: 40px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 30px;
        }
        
        .footer-section h3 {
            color: #d1e7dd;
            margin-bottom: 20px;
            font-size: 1.3rem;
        }
        
        .footer-section p, .footer-section li {
            margin-bottom: 10px;
            opacity: 0.9;
        }
        
        .footer-section ul {
            list-style-type: none;
            padding-left: 0;
        }
        
        .footer-section a {
            color: #d1e7dd;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer-section a:hover {
            color: #ffffff;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.8;
            font-size: 0.9rem;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
                gap: 15px;
            }
            
            .logo {
                flex-direction: column;
                text-align: center;
            }
            
            .logo-img {
                height: 60px;
            }
            
            .hero-content h2 {
                font-size: 2rem;
            }
            
            .hero-content p {
                font-size: 1rem;
            }
            
            .highlight {
                font-size: 1.1rem;
                padding: 10px 20px;
            }
            
            .age-groups {
                flex-direction: column;
                align-items: center;
            }
            
            .form-container {
                padding: 25px;
            }
            
            .whatsapp-float {
                width: 50px;
                height: 50px;
                font-size: 1.7rem;
                bottom: 20px;
                right: 20px;
            }
            
            .hours-grid {
                grid-template-columns: 1fr;
            }
            
            .map-container {
                height: 350px;
            }
            
            .whatsapp-grid {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 480px) {
            .logo-img {
                height: 50px;
            }
            
            .logo-text h1 {
                font-size: 1.5rem;
            }
            
            .contact-info {
                flex-direction: column;
                gap: 10px;
            }
            
            .map-container {
                height: 300px;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <!-- Logo MQirad - Updated to your JPEG file -->
                    <img src="https://i.ibb.co/1fv1Q1gt/Gemini-Generated-Image-cuor7cuor7cuor7c.png" alt="M-Qirad Logo" class="logo-img" border="0">
                    <div class="logo-text">
                        <h1>M-QIRAD</h1>
                        <p>Perundingan Kewangan Profesional</p>
                    </div>
                </div>
                <div class="contact-info">
                    <div class="contact-item">
                        <i class="fas fa-phone-alt contact-icon"></i>
                        <span>+6010-658 3343</span>
                    </div>
                    <div class="contact-item">
                        <i class="fas fa-envelope contact-icon"></i>
                        <span>officialmqirad@gmail.com</span>
                    </div>
                </div>
            </div>
        </div>
    </header>
    
    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <h2>PERUNDINGAN KEWANGAN PROFESIONAL</h2>
                <p>Kami Menawarkan Perkhidmatan Penyelesaian Menggunakan Caruman KWSP Anda.<br>
                Tanpa Bayaran Pendahuluan Dan Tanpa Bebanan Komitmen Bulanan.</p>
                <div class="highlight">
                    Kadar Kelulusan 99.9% Lulus
                </div>
            </div>
        </div>
    </section>
    
    <!-- Company Information -->
    <section class="company-info">
        <div class="container">
            <h2 class="section-title">Tentang M-Qirad</h2>
            <div class="company-details">
                <h3>MILANO ENTERPRISE SDN BHD (207404-D)</h3>
                <p>ATAU LEBIH DIKENALI SEBAGAI MQIRAD ADALAH SEBUAH SYARIKAT KREDIT KOMUNITI PEMBERI PINJAMAN WANG BERLESEN YANG BERDAFTAR DI BAWAH AKTA PEMBERI PINJAM WANG 1951.</p>
                <p>KAMI MEMBERIKAN KEMUDAHAN PEMBIAYAAN KHAS UNTUK INDIVIDU BERUMUR:</p>
                
                <div class="age-groups">
                    <div class="age-group">
                        <h4>53 - 55</h4>
                        <p>Tahun</p>
                    </div>
                    <div class="age-group">
                        <h4>58 - 60</h4>
                        <p>Tahun</p>
                    </div>
                </div>
                
                <p style="margin-top: 20px;">YANG MEMERLUKAN TUNAI SEGERA. PERMOHONAN BOLEH DIBUAT <strong>SECARA ATAS TALIAN</strong>.</p>
                
                <div style="background-color: #f5f9f7; padding: 15px; border-radius: 5px; margin-top: 20px; border-left: 4px solid #1a472a;">
                    <h4 style="color: #a83232;">ADA KAH MQIRAD BERKAITAN DENGAN PIHAK KWSP?</h4>
                    <p style="font-weight: bold; color: #a83232; font-size: 1.2rem;">TIDAK. MQIRAD BUKAN WAKIL ATAU EJEN DARI PIHAK KWSP</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Benefits Section -->
    <section class="benefits">
        <div class="container">
            <h2 class="section-title">Manfaat Pinjaman KWSP Yang Kami Tawarkan</h2>
            <div class="benefits-grid">
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="far fa-calendar-check"></i>
                    </div>
                    <h3>Tiada Bayaran Bulanan</h3>
                    <p>Tiada bayaran bulanan sehingga 24 bulan. Anda hanya perlu membayar balik selepas pengeluaran KWSP diterima.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-money-check-alt"></i>
                    </div>
                    <h3>Tiada Bayaran Pendahuluan</h3>
                    <p>Tiada bayaran pendahuluan atau caj tersembunyi. Semua kos dijelaskan dengan telus dalam perjanjian.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-file-contract"></i>
                    </div>
                    <h3>Perjanjian Yang Jelas Dan Sah</h3>
                    <p>Mempunyai surat perjanjian yang jelas dan sah dari segi undang-undang untuk melindungi hak kedua-dua pihak.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Data Peribadi Terlindung</h3>
                    <p>Semua data peribadi anda dilindungi dengan selamat dan tidak akan dikongsi dengan pihak ketiga tanpa kebenaran.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Kadar Kelulusan Tinggi</h3>
                    <p>Kadar kelulusan 99.9% dengan proses yang pantas dan mudah untuk mereka yang layak.</p>
                </div>
                
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-hand-holding-usd"></i>
                    </div>
                    <h3>Kaedah Pembayaran Semula</h3>
                    <p>Bayaran semula oleh peminjam perlu dijelaskan kepada pihak syarikat setelah pengeluaran KWSP diterima.</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Text Testimonials -->
    <section class="testimonials">
        <div class="container">
            <h2 class="section-title">Testimoni Pelanggan Berjaya</h2>
            <div class="testimonial-grid">
                <div class="testimonial-card">
                    <div class="customer-name">
                        <i class="fas fa-user-circle"></i>
                        <span>Encik Ahmad, 55 Tahun</span>
                    </div>
                    <p>"Sangat berpuas hati dengan perkhidmatan M-Qirad. Proses pantas dan tiada bayaran pendahuluan. Wang tunai diterima dalam masa 3 hari selepas permohonan."</p>
                </div>
                
                <div class="testimonial-card">
                    <div class="customer-name">
                        <i class="fas fa-user-circle"></i>
                        <span>Puan Siti, 59 Tahun</span>
                    </div>
                    <p>"Sebagai pesara, saya perlukan tunai segera untuk perbelanjaan perubatan. M-Qirad bantu saya dengan pinjaman menggunakan KWSP tanpa komitmen bulanan. Sangat disyorkan!"</p>
                </div>
                
                <div class="testimonial-card">
                    <div class="customer-name">
                        <i class="fas fa-user-circle"></i>
                        <span>Encik Raju, 54 Tahun</span>
                    </div>
                    <p>"Walaupun saya dalam senarai hitam bank, permohonan saya diluluskan oleh M-Qirad. Proses sangat mudah dan semua terma dijelaskan dengan jelas."</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- NEW: WhatsApp Image Testimonials -->
    <section class="whatsapp-testimonials">
        <div class="container">
            <h2 class="section-title">Bukti Kejayaan Pelanggan Kami</h2>
            <p style="text-align: center; max-width: 800px; margin: 0 auto 30px; color: #333333;">
                Berikut adalah bukti transaksi sebenar daripada pelanggan kami yang telah berjaya menerima pinjaman KWSP melalui M-Qirad. 
                Setiap gambar menunjukkan transaksi bank yang berjaya dihantar terus ke akaun pelanggan.
            </p>
            
            <div class="whatsapp-grid">
                <!-- Testimonial 1 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Rohani</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/qLcyVsXD/Whats-App-Image-2025-12-16-at-15-58-50-1.jpg" alt="WhatsApp Testimonial 1" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM5,000.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>07 Oct 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Rama</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/Q1zmQv5/Whats-App-Image-2025-12-16-at-15-57-19.jpg" alt="WhatsApp Testimonial 2" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM20,000.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>03 Feb 2024</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Shamsurill...</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/kgm6b093/Whats-App-Image-2025-12-16-at-16-00-08.jpg" alt="WhatsApp Testimonial 3" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM20,000.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>01 Aug 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 4 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Aishah</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/d0XyBktn/Whats-App-Image-2025-12-16-at-15-57-16.jpg" alt="WhatsApp Testimonial 4" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM5,700.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>04 Dec 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 5 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Jeffry</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/N6335JL9/Whats-App-Image-2025-12-16-at-15-57-18.jpg" alt="WhatsApp Testimonial 5" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM16,000.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>02 Sep 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 6 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Mohd Azlan</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/svMx5FrF/Whats-App-Image-2025-12-16-at-15-58-50.jpg" alt="WhatsApp Testimonial 6" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM10,000.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>02 Oct 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 7 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Mohd Badlishah</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/Pf26WBx/Whats-App-Image-2025-12-16-at-15-57-17-1.jpg" alt="WhatsApp Testimonial 7" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM30,097.81</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>29 May 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 8 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Shahmaru</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/RGQwsD98/Whats-App-Image-2025-12-16-at-15-57-17.jpg" alt="WhatsApp Testimonial 8" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM25,000.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>01 Dec 2025</span>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 9 -->
                <div class="whatsapp-card">
                    <div class="whatsapp-header">
                        <i class="fab fa-whatsapp whatsapp-icon"></i>
                        <div class="whatsapp-customer">Fazlita</div>
                    </div>
                    <div class="whatsapp-image-container">
                        <img src="https://i.ibb.co/kgN51pdw/Whats-App-Image-2025-12-16-at-15-58-49.jpg" alt="WhatsApp Testimonial 9" class="whatsapp-image" style="max-height: 250px;">
                        <!-- Replace the src above with your actual image URL -->
                    </div>
                    <div class="whatsapp-info">
                        <div class="whatsapp-amount">RM7,600.00</div>
                        <div class="whatsapp-date">
                            <i class="far fa-calendar"></i>
                            <span>01 Oct 2025</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <div style="text-align: center; margin-top: 40px; padding: 20px; background-color: #f5f9f7; border-radius: 10px; border: 1px solid #1a472a;">
                <h3 style="color: #1a472a; margin-bottom: 15px;">Setiap Transaksi Adalah Bukti Kejayaan Kami</h3>
                <p style="color: #333333; max-width: 800px; margin: 0 auto;">
                    Setiap gambar di atas adalah bukti sebenar transaksi pelanggan kami yang berpuas hati dengan perkhidmatan M-Qirad. 
                    Kami berbangga dapat membantu ramai pelanggan mendapatkan pinjaman KWSP dengan mudah, pantas dan telus.
                </p>
            </div>
        </div>
    </section>
    
    <!-- Google Maps Location -->
    <section class="location">
        <div class="container">
            <h2 class="section-title">Lokasi Kami</h2>
            
            <div class="map-container">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3983.11032666338!2d101.57393557567582!3d3.3229075520584845!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x31cc4380cd12ee03%3A0x5fe0a789b5d066d8!2sKredit%20Komuniti%20M-Qirad%20-%20Milano%20Enterprise%20Sdn.%20Bhd.!5e0!3m2!1sen!2smy!4v1765942703691!5m2!1sen!2smy" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
            </div>
            
            <div class="location-info">
                <h3>Alamat Pejabat Kami</h3>
                <p><i class="fas fa-map-marker-alt"></i> Kredit Komuniti M-Qirad - Milano Enterprise Sdn. Bhd.</p>
                <p><i class="fas fa-map-pin"></i> 13A, Jalan Bandar Rawang 2, Pusat Bandar Rawang, 48000 Rawang, Selangor</p>
                <p><i class="fas fa-phone"></i> <a href="tel:+60106583343">+6010-658 3343</a></p>
                <p><i class="fas fa-clock"></i> Isnin - Jumaat: 9:30 pagi - 5:30 petang | Sabtu: 9:30 pagi - 2:00 petang</p>
            </div>
        </div>
    </section>
    
    <!-- Operating Hours -->
    <section class="operating-hours">
        <div class="container">
            <h2 class="section-title">Waktu Operasi Kami</h2>
            <div class="hours-container">
                <p style="text-align: center; margin-bottom: 20px; color: #1a472a; font-weight: 600;">
                    Kami sedia membantu anda pada waktu operasi berikut:
                </p>
                <div class="hours-grid">
                    <div class="hours-day">
                        <div class="day-name">
                            <i class="fas fa-calendar-day"></i>
                            <span>Isnin - Jumaat</span>
                        </div>
                        <div class="day-time">9:30 pagi - 5:30 petang</div>
                    </div>
                    
                    <div class="hours-day special">
                        <div class="day-name">
                            <i class="fas fa-calendar-day"></i>
                            <span>Sabtu</span>
                        </div>
                        <div class="day-time">9:30 pagi - 2:00 petang</div>
                    </div>
                    
                    <div class="hours-day closed">
                        <div class="day-name">
                            <i class="fas fa-calendar-times"></i>
                            <span>Ahad & Cuti Umum</span>
                        </div>
                        <div class="day-time">Cuti</div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Application Form -->
    <section class="application">
        <div class="container">
            <h2 class="section-title">Permohonan Atas Talian Dibuka</h2>
            <div class="form-container">
                <p style="text-align: center; margin-bottom: 30px; font-size: 1.1rem; color: #1a472a; font-weight: bold;">
                    Dokumen Ringkas, Kelulusan Segera, Proses Cepat, Dan Mudah
                </p>
                
                <form id="loanApplicationForm">
                    <div class="form-group">
                        <label for="name">NAMA:</label>
                        <input type="text" id="name" name="name" required placeholder="Masukkan nama penuh anda">
                    </div>
                    
                    <div class="form-group">
                        <label for="phone">NO TELEFON:</label>
                        <input type="tel" id="phone" name="phone" required placeholder="Contoh: 012-345 6789">
                    </div>
                    
                    <div class="form-group">
                        <label for="state">NEGERI:</label>
                        <select id="state" name="state" required>
                            <option value="">Pilih Negeri</option>
                            <option value="johor">Johor</option>
                            <option value="kedah">Kedah</option>
                            <option value="kelantan">Kelantan</option>
                            <option value="melaka">Melaka</option>
                            <option value="negeri-sembilan">Negeri Sembilan</option>
                            <option value="pahang">Pahang</option>
                            <option value="perak">Perak</option>
                            <option value="perlis">Perlis</option>
                            <option value="pulau-pinang">Pulau Pinang</option>
                            <option value="selangor">Selangor</option>
                            <option value="terengganu">Terengganu</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="birthdate">TARIKH LAHIR:</label>
                        <div class="calendar-container">
                            <input type="date" id="birthdate" name="birthdate" required>
                            <i class="far fa-calendar-alt"></i>
                        </div>
                        <small style="color: #666; font-size: 0.85rem; margin-top: 5px; display: block;">
                            * Anda boleh memilih mana-mana tarikh lahir menggunakan kalendar
                        </small>
                    </div>
                    
                    <div class="form-group">
                        <label for="kwsp_amount">JUMLAH SIMPANAN KWSP:</label>
                        <input type="text" id="kwsp_amount" name="kwsp_amount" required placeholder="Contoh: RM30,000">
                    </div>
                    
                    <div class="requirements">
                        <h3>KELAYAKAN PEMOHON:</h3>
                        <ul>
                            <li>Kelayakan khas umur 53, 54, 55 & 58, 59, 60 tahun</li>
                            <li>Mempunyai simpanan KWSP Akaun 1 atau Akaun Emas (Simpanan minimum RM30K)</li>
                            <li>Blacklist/CTOSS/Bankruptcy/AKPK Layak</li>
                            <li>Bekerja / Tidak Bekerja Layak</li>
                            <li>Seluruh Semenanjung Malaysia (Kecuali Sabah, Sarawak)</li>
                        </ul>
                    </div>
                    
                    <button type="submit" class="submit-btn">
                        <i class="fas fa-paper-plane"></i> HANTAR PERMOHONAN SEKARANG
                    </button>
                </form>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>M-QIRAD</h3>
                    <p>Milano Enterprise Sdn Bhd (207404-D)</p>
                    <p>Syarikat Kredit Komuniti Pemberi Pinjaman Wang Berlesen</p>
                    <p>Berdaftar di bawah Akta Pemberi Pinjam Wang 1951</p>
                </div>
                
                <div class="footer-section">
                    <h3>Hubungi Kami</h3>
                    <p><i class="fas fa-phone"></i> <a href="tel:+60106583343">+6010-658 3343</a></p>
                    <p><i class="fas fa-envelope"></i> <a href="mailto:officialmqirad@gmail.com">officialmqirad@gmail.com</a></p>
                    <p><i class="fab fa-whatsapp"></i> <a href="https://wa.me/60106583343" target="_blank">+6010-658 3343 (WhatsApp)</a></p>
                </div>
                
                <div class="footer-section">
                    <h3>Waktu Operasi</h3>
                    <p><i class="far fa-clock"></i> Isnin - Jumaat: 9:30 pagi - 5:30 petang</p>
                    <p><i class="far fa-clock"></i> Sabtu: 9:30 pagi - 2:00 petang</p>
                    <p><i class="fas fa-door-closed"></i> Ahad & Cuti Umum: Cuti</p>
                </div>
                
                <div class="footer-section">
                    <h3>Lokasi Kami</h3>
                    <p><i class="fas fa-map-marker-alt"></i> 13A, Jalan Bandar Rawang 2/1E</p>
                    <p>Pusat Bandar Rawang</p>
                    <p>48000 Rawang, Selangor</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 M-Qirad. Hak Cipta Terpelihara.</p>
            </div>
        </div>
    </footer>
    
    <!-- WhatsApp Floating Button -->
    <a href="https://wa.me/60106583343" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>
    
    <script>
        // Function to calculate age
        function calculateAge(birthDate) {
            const today = new Date();
            let age = today.getFullYear() - birthDate.getFullYear();
            const monthDiff = today.getMonth() - birthDate.getMonth();
            if (monthDiff < 0 || (monthDiff === 0 && today.getDate() < birthDate.getDate())) {
                age--;
            }
            return age;
        }
        
        // Initialize the date input when page loads
        document.addEventListener('DOMContentLoaded', function() {
            const birthdateInput = document.getElementById('birthdate');
            
            // Set a default date (e.g., 55 years ago) for better UX
            const defaultDate = new Date();
            defaultDate.setFullYear(defaultDate.getFullYear() - 55);
            
            // Format date for input (YYYY-MM-DD)
            const formatDate = (date) => {
                const year = date.getFullYear();
                const month = String(date.getMonth() + 1).padStart(2, '0');
                const day = String(date.getDate()).padStart(2, '0');
                return `${year}-${month}-${day}`;
            };
            
            // Remove any min/max restrictions to allow all dates
            birthdateInput.removeAttribute('min');
            birthdateInput.removeAttribute('max');
            
            // Set default value for better UX
            birthdateInput.value = formatDate(defaultDate);
            
            // Ensure calendar icon is visible
            birthdateInput.addEventListener('focus', function() {
                this.showPicker && this.showPicker();
            });
        });
        
        // Form submission handler
        document.getElementById('loanApplicationForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form values
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            const state = document.getElementById('state').value;
            const birthdate = document.getElementById('birthdate').value;
            const kwspAmount = document.getElementById('kwsp_amount').value;
            
            // Basic validation
            if (!name || !phone || !state || !birthdate || !kwspAmount) {
                alert('Sila isi semua maklumat yang diperlukan.');
                return;
            }
            
            // Calculate age from birthdate
            const birthDate = new Date(birthdate);
            const age = calculateAge(birthDate);
            
            // Check age eligibility
            const eligibleAges = [53, 54, 55, 58, 59, 60];
            const isEligibleAge = eligibleAges.includes(age);
            
            // Check KWSP amount
            const kwspValue = parseFloat(kwspAmount.replace(/[^0-9.-]+/g, ""));
            const isEligibleKwsp = kwspValue >= 30000;
            
            // Check if within operating hours
            const now = new Date();
            const day = now.getDay(); // 0 = Sunday, 1 = Monday, ..., 6 = Saturday
            const hour = now.getHours();
            const minute = now.getMinutes();
            
            let isOperatingHours = false;
            let message = "";
            
            if (day >= 1 && day <= 5) { // Monday to Friday
                if ((hour > 9 || (hour === 9 && minute >= 30)) && (hour < 17 || (hour === 17 && minute <= 30))) {
                    isOperatingHours = true;
                } else {
                    message = "Waktu operasi kami pada hari bekerja adalah 9:30 pagi hingga 5:30 petang.";
                }
            } else if (day === 6) { // Saturday
                if ((hour > 9 || (hour === 9 && minute >= 30)) && (hour < 14 || (hour === 14 && minute <= 0))) {
                    isOperatingHours = true;
                } else {
                    message = "Waktu operasi kami pada hari Sabtu adalah 9:30 pagi hingga 2:00 petang.";
                }
            } else { // Sunday or public holiday
                message = "Kami bercuti pada hari Ahad dan cuti umum. Permohonan anda akan diproses pada hari bekerja berikutnya.";
            }
            
            // Format date for display
            const formattedDate = new Date(birthdate).toLocaleDateString('ms-MY', {
                day: '2-digit',
                month: '2-digit',
                year: 'numeric'
            });
            
            // Success message with WhatsApp option
            const whatsappMsg = `Hai, saya ${name}. Saya baru sahaja menghantar permohonan pinjaman KWSP melalui laman web M-Qirad. No telefon: ${phone}, Negeri: ${state}, Umur: ${age} tahun, Tarikh Lahir: ${formattedDate}, Simpanan KWSP: ${kwspAmount}. Sila hubungi saya untuk maklumat lanjut.`;
            const encodedMsg = encodeURIComponent(whatsappMsg);
            const whatsappLink = `https://wa.me/60106583343?text=${encodedMsg}`;
            
            // Age eligibility check
            let eligibilityMessage = "";
            if (!isEligibleAge) {
                eligibilityMessage = `\n\nPERHATIAN: Umur anda (${age} tahun) tidak termasuk dalam kumpulan umur yang layak (53-55 & 58-60 tahun). Walau bagaimanapun, kami masih akan memproses permohonan anda dan menghubungi anda untuk perbincangan lanjut.`;
            }
            
            if (!isEligibleKwsp) {
                eligibilityMessage += `\n\nPERHATIAN: Simpanan KWSP anda (RM${kwspValue.toLocaleString()}) adalah di bawah minimum RM30,000. Walau bagaimanapun, kami masih akan memproses permohonan anda dan menghubungi anda untuk perbincangan lanjut.`;
            }
            
            let alertMessage = `Terima kasih ${name}! Permohonan anda telah berjaya dihantar.\nUmur: ${age} tahun\nTarikh Lahir: ${formattedDate}\n${eligibilityMessage}\n\n`;
            
            if (!isOperatingHours && message) {
                alertMessage += `${message}\n\n`;
            }
            
            alertMessage += "Klik OK untuk terus berhubung dengan kami melalui WhatsApp atau Cancel untuk teruskan.";
            
            const userChoice = confirm(alertMessage);
            
            if (userChoice) {
                window.open(whatsappLink, '_blank');
            } else {
                const followUpMsg = isOperatingHours 
                    ? 'Wakil kami akan menghubungi anda di ' + phone + ' dalam masa 24 jam bekerja.'
                    : message + ' Wakil kami akan menghubungi anda pada hari bekerja berikutnya.';
                alert(followUpMsg);
            }
            
            // Reset form
            document.getElementById('loanApplicationForm').reset();
        });
    </script>
</body>
</html>

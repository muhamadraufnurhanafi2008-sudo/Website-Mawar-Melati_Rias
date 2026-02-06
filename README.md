# Website-Mawar-Melati_Rias
Website untuk mengetahui lebih lanjut tentang Jasa Rias dan Dekorasi
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Glamour Deco & Makeup - Dekorasi & Tata Rias Terbaik</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #f5f7fa, #c3cfe2);
            color: #333;
        }
        header {
            background: rgba(255, 255, 255, 0.9);
            padding: 20px;
            text-align: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            animation: fadeIn 1s ease-in;
        }
        h1 {
            color: #e91e63;
            font-size: 2.5em;
            margin: 0;
        }
        .hero {
            background: url('https://source.unsplash.com/featured/?wedding,decoration') no-repeat center/cover;
            height: 70vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
        }
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0,0,0,0.4);
        }
        .hero h2 {
            font-size: 3em;
            z-index: 1;
            position: relative;
            animation: slideUp 1.5s ease-out;
        }
        .hero p {
            font-size: 1.2em;
            z-index: 1;
            position: relative;
        }
        .cta-button {
            background: #e91e63;
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s;
        }
        .cta-button:hover {
            transform: scale(1.1);
        }
        section {
            padding: 50px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        .services {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        .service {
            background: white;
            border-radius: 10px;
            padding: 20px;
            margin: 10px;
            width: 300px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }
        .service:hover {
            transform: translateY(-10px);
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .gallery img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 10px;
            transition: opacity 0.3s;
        }
        .gallery img:hover {
            opacity: 0.8;
        }
        .testimonials {
            background: #f9f9f9;
            padding: 40px;
            border-radius: 10px;
        }
        .testimonial {
            margin: 20px 0;
            font-style: italic;
        }
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes slideUp {
            from { transform: translateY(50px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }
        @media (max-width: 768px) {
            .hero h2 { font-size: 2em; }
            .services { flex-direction: column; }
        }
    </style>
</head>
<body>
    <header>
        <h1>Glamour Deco & Makeup</h1>
        <p>Dekorasi dan Tata Rias untuk Acara Impian Anda</p>
    </header>

    <section class="hero">
        <div>
            <h2>Buat Acara Anda Berkesan Abadi</h2>
            <p>Layanan dekorasi mewah dan tata rias profesional untuk pernikahan, ulang tahun, dan acara spesial lainnya.</p>
            <a href="#contact" class="cta-button">Hubungi Kami Sekarang</a>
        </div>
    </section>

    <section id="services">
        <h2>Layanan Kami</h2>
        <div class="services">
            <div class="service">
                <h3>Dekorasi Acara</h3>
                <p>Desain dekorasi yang elegan dan kreatif untuk berbagai tema acara.</p>
            </div>
            <div class="service">
                <h3>Tata Rias Wajah</h3>
                <p>Makeup profesional untuk pengantin, model, atau acara formal.</p>
            </div>
            <div class="service">
                <h3>Paket Lengkap</h3>
                <p>Kombinasi dekorasi dan tata rias dengan harga terjangkau.</p>
            </div>
        </div>
    </section>

    <section id="gallery">
        <h2>Galeri Karya Kami</h2>
        <div class="gallery">
            <img src="https://source.unsplash.com/featured/?wedding,flowers" alt="Dekorasi Pernikahan">
            <img src="https://source.unsplash.com/featured/?makeup,bride" alt="Tata Rias Pengantin">
            <img src="https://source.unsplash.com/featured/?party,decoration" alt="Dekorasi Pesta">
            <img src="https://source.unsplash.com/featured/?beauty,makeup" alt="Makeup Artist">
        </div>
    </section>

    <section id="testimonials" class="testimonials">
        <h2>Testimoni Klien</h2>
        <div class="testimonial">
            <p>"Dekorasi dan makeup-nya luar biasa! Acara pernikahan saya jadi tak terlupakan." - Sari, Pengantin</p>
        </div>
        <div class="testimonial">
            <p>"Tim profesional dan hasilnya memukau. Sangat recommended!" - Andi, Event Organizer</p>
        </div>
    </section>

    <section id="contact">
        <h2>Hubungi Kami</h2>
        <p>Email: info@glamourdeco.com | Telepon: +62 812-3456-7890 | Alamat: Jakarta, Indonesia</p>
        <a href="mailto:info@glamourdeco.com" class="cta-button">Kirim Email</a>
    </section>

    <footer>
        <p>&copy; 2023 Glamour Deco & Makeup. Semua Hak Dilindungi.</p>
    </footer>
</body>
</html>

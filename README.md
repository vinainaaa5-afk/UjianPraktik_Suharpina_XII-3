
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Lilac Elegan</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <nav class="navbar navbar-expand-lg navbar-dark fixed-top custom-navbar">
        <div class="container">
            <a class="navbar-brand" href="#">**[Nama Anda]**</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#hero">Beranda</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#about">Tentang</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#portfolio">Portofolio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#contact">Kontak</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <section id="hero" class="d-flex align-items-center justify-content-center text-center custom-hero">
        <div class="container">
            <h1 class="display-3 fw-bold custom-title">Halo, Saya [Nama Anda]</h1>
            <p class="lead custom-text">Seorang **[Gelar/Profesi Anda]** yang fokus pada desain elegan dan fungsional.</p>
            <a href="#portfolio" class="btn btn-lg custom-btn mt-3">Lihat Karya Saya</a>
        </div>
    </section>

    <section id="about" class="py-5 custom-section">
        <div class="container">
            <div class="row">
                <div class="col-lg-6 mb-4 mb-lg-0">
                    <h2 class="display-5 fw-bold custom-heading mb-4">Tentang Saya 🎨</h2>
                    <p class="custom-text">Saya memiliki pengalaman dalam **[Sebutkan Keahlian Utama, misal: Web Development / Graphic Design]** dan selalu berusaha menciptakan solusi yang tidak hanya indah tetapi juga efisien. Prinsip saya adalah kesederhanaan adalah kunci keeleganan.</p>
                    <p class="custom-text">Beberapa keahlian saya meliputi: **HTML, CSS, JavaScript, Bootstrap, [Keahlian Lain]**.</p>
                </div>
                <div class="col-lg-6 text-center">
                    <div class="custom-profile-pic mx-auto">
                        
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
/* Definisi Warna Cream Kustom */
:root {
    --cream-primary: #F8F0E3;   /* Cream utama, terang */
    --cream-secondary: #EADBC8; /* Cream sedikit lebih gelap/hangat */
    --cream-dark: #C7B7A7;      /* Cream gelap untuk aksen */
    --text-dark: #4A4A4A;       /* Teks gelap untuk kontras */
    --text-light: #6C6C6C;      /* Teks sedikit lebih terang */
}

body {
    font-family: 'Roboto', sans-serif; /* Font bersih untuk body */
    background-color: var(--cream-primary);
    color: var(--text-dark);
    padding-top: 60px; /* Agar konten tidak tertutup fixed-top navbar */
    line-height: 1.7; /* Meningkatkan keterbacaan */
}

h1, h2, h3, h4, h5, h6 {
    font-family: 'Playfair Display', serif; /* Font elegan untuk judul */
    color: var(--text-dark);
}

/* --- Navigasi --- */
.custom-navbar {
    background-color: var(--cream-primary) !important;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05); /* Shadow lembut */
    padding: 1rem 0;
}

.custom-navbar .navbar-brand {
    color: var(--text-dark) !important;
    font-weight: 700;
    font-size: 1.6rem;
    letter-spacing: 0.5px;
}

.custom-navbar .nav-link {
    color: var(--text-light) !important;
    margin-left: 25px;
    font-size: 1.05rem;
    position: relative;
    transition: color 0.3s ease;
}

.custom-navbar .nav-link::after {
    content: '';
    position: absolute;
    width: 0%;
    height: 2px;
    background-color: var(--cream-dark);
    left: 0;
    bottom: -5px;
    transition: width 0.3s ease;
}

.custom-navbar .nav-link:hover::after,
.custom-navbar .nav-link.active::after {
    width: 100%;
}

.custom-navbar .nav-link:hover,
.custom-navbar .nav-link.active {
    color: var(--cream-dark) !important;
}

/* --- Bagian Hero --- */
.custom-hero {
    min-height: 100vh;
    background: linear-gradient(135deg, var(--cream-primary), var(--cream-secondary));
    color: var(--text-dark);
    padding: 100px 0;
}

.custom-title {
    font-size: 4rem;
    font-weight: 700;
    letter-spacing: 1px;
    line-height: 1.2;
}

.custom-text {
    max-width: 700px;
    margin: 20px auto 0;
    font-size: 1.2rem;
    color: var(--text-light);
}

.custom-btn {
    background-color: var(--cream-dark);
    border: 1px solid var(--cream-dark);
    padding: 12px 35px;
    border-radius: 5px; /* Sudut sedikit membulat */
    transition: background-color 0.3s ease, transform 0.2s ease, border-color 0.3s ease;
    color: white; /* Teks putih agar kontras */
    font-weight: 500;
    letter-spacing: 0.5px;
    text-transform: uppercase;
}

.custom-btn:hover {
    background-color: #B0A090; /* Sedikit lebih gelap saat hover */
    border-color: #B0A090;
    transform: translateY(-3px);
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    color: white;
}

/* --- Bagian Umum (Section) --- */
.custom-section {
    padding: 80px 0;
    border-bottom: 1px solid #E5E5E5; /* Garis pemisah halus */
}

.custom-heading {
    color: var(--cream-dark);
    font-size: 3rem;
    margin-bottom: 2.5rem;
}

/* --- Foto Profil --- */
.custom-profile-pic {
    width: 280px;
    height: 280px;
    border-radius: 50%;
    background-color: var(--cream-secondary); /* Warna latar untuk placeholder */
    border: 6px solid var(--cream-dark);
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden; /* Penting jika ada gambar di dalamnya */
    box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
}

.custom-profile-pic img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Media Queries untuk responsivitas */
@media (max-width: 768px) {
    .custom-title {
        font-size: 3rem;
    }
    .custom-heading {
        font-size: 2.5rem;
    }
    .custom-hero {
        padding: 80px 0;
    }
    .custom-profile-pic {
        width: 200px;
        height: 200px;
        margin-bottom: 2rem !important; /* Spasi di mobile */
    }
}

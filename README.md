# Portfolio Website

Website portfolio profesional yang responsive, modern, dan mudah di-maintenance. Dibangun dengan HTML5, CSS3, dan JavaScript vanilla untuk performa optimal dan kemudahan editing.

## 🚀 Fitur

- **Responsive Design** - Tampil sempurna di desktop, tablet, dan mobile
- **Modern UI/UX** - Desain clean dan professional dengan animasi smooth
- **SEO Optimized** - Meta tags lengkap untuk search engine optimization
- **Fast Loading** - Optimized untuk performa terbaik
- **Easy Maintenance** - Struktur kode yang jelas dan dokumentasi lengkap
- **GitHub Pages Ready** - Siap untuk hosting gratis di GitHub Pages

## 📁 Struktur File

```
portfolio-website/
├── index.html          # Halaman utama
├── styles.css          # Styling CSS
├── script.js           # JavaScript functionality
├── _config.yml         # Konfigurasi GitHub Pages
├── 404.html           # Halaman error 404
├── CNAME              # Custom domain (opsional)
└── README.md          # Dokumentasi
```

## 🛠️ Setup & Deployment

### 1. Persiapan Repository

1. Buat repository baru di GitHub dengan nama `[username].github.io`
2. Clone repository ke komputer Anda:
   ```bash
   git clone https://github.com/[username]/[username].github.io.git
   cd [username].github.io
   ```

### 2. Upload Files

1. Copy semua file dari project ini ke folder repository
2. Commit dan push ke GitHub:
   ```bash
   git add .
   git commit -m "Initial portfolio setup"
   git push origin main
   ```

### 3. Aktifkan GitHub Pages

1. Pergi ke repository di GitHub
2. Klik tab **Settings**
3. Scroll ke bagian **Pages**
4. Di **Source**, pilih **Deploy from a branch**
5. Pilih branch **main** dan folder **/ (root)**
6. Klik **Save**

Website Anda akan tersedia di: `https://[username].github.io`

## ✏️ Cara Edit Konten

### 1. Informasi Personal

Edit file `index.html` dan ganti placeholder berikut:

```html
<!-- Ganti [Nama Anda] dengan nama Anda -->
<title>[Nama Anda] - Portfolio</title>

<!-- Di hero section -->
<h1 class="hero-title">Hi, I'm <span class="highlight">[Nama Anda]</span></h1>

<!-- Di about section -->
<p>I'm a passionate web developer with [X] years of experience...</p>
```

### 2. Informasi Kontak

Update informasi kontak di section contact:

```html
<!-- Email -->
<span>your.email@example.com</span>

<!-- Phone -->
<span>+62 812-3456-7890</span>

<!-- Location -->
<span>Jakarta, Indonesia</span>

<!-- Social Media Links -->
<a href="https://linkedin.com/in/yourprofile" class="social-link">
  <a href="https://github.com/yourusername" class="social-link">
    <a href="https://twitter.com/yourusername" class="social-link"></a></a
></a>
```

### 3. Skills & Technologies

Edit skills di section skills:

```html
<div class="skill-items">
  <span class="skill-item">HTML5</span>
  <span class="skill-item">CSS3</span>
  <span class="skill-item">JavaScript</span>
  <!-- Tambah atau hapus skill sesuai kebutuhan -->
</div>
```

### 4. Projects

Update project cards di section projects:

```html
<div class="project-card">
  <div class="project-content">
    <h3>Nama Project</h3>
    <p>Deskripsi project Anda...</p>
    <div class="project-tech">
      <span>React</span>
      <span>Node.js</span>
    </div>
    <div class="project-links">
      <a href="https://yourproject.com" class="project-link">
        <i class="fas fa-external-link-alt"></i> Live Demo
      </a>
      <a href="https://github.com/yourusername/project" class="project-link">
        <i class="fab fa-github"></i> GitHub
      </a>
    </div>
  </div>
</div>
```

## 🎨 Customization

### 1. Mengubah Warna

Edit file `styles.css` dan ubah variabel warna:

```css
/* Primary colors */
:root {
  --primary-color: #667eea;
  --secondary-color: #764ba2;
  --text-color: #333;
  --bg-color: #ffffff;
}
```

### 2. Mengubah Font

Ganti font di bagian atas `styles.css`:

```css
/* Import font baru dari Google Fonts */
@import url("https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700&display=swap");

/* Update font-family */
body {
  font-family: "YourFont", sans-serif;
}
```

### 3. Menambah Section Baru

1. Tambah section di `index.html`:

```html
<section id="new-section" class="new-section">
  <div class="container">
    <h2 class="section-title">Section Title</h2>
    <!-- Konten section -->
  </div>
</section>
```

2. Tambah styling di `styles.css`:

```css
.new-section {
  padding: 5rem 0;
  background: #f8f9fa;
}
```

3. Update navigation di `index.html`:

```html
<a href="#new-section" class="nav-link">New Section</a>
```

## 📱 Responsive Design

Website sudah responsive untuk semua device:

- **Desktop**: 1200px+
- **Tablet**: 768px - 1199px
- **Mobile**: < 768px

Untuk menyesuaikan breakpoint, edit media queries di `styles.css`:

```css
@media (max-width: 768px) {
  /* Mobile styles */
}

@media (max-width: 480px) {
  /* Small mobile styles */
}
```

## 🚀 Performance Tips

### 1. Optimize Images

- Gunakan format WebP untuk gambar
- Compress gambar sebelum upload
- Gunakan lazy loading untuk gambar

### 2. Minify Files

Untuk production, minify CSS dan JS:

```bash
# Install tools
npm install -g clean-css-cli uglify-js

# Minify CSS
cleancss -o styles.min.css styles.css

# Minify JS
uglifyjs script.js -o script.min.js
```

### 3. Enable Caching

Tambahkan meta tags untuk caching:

```html
<meta http-equiv="Cache-Control" content="max-age=31536000" />
```

## 🔧 Troubleshooting

### GitHub Pages Tidak Update

1. Pastikan file sudah di-commit dan di-push
2. Tunggu 5-10 menit untuk GitHub Pages update
3. Clear cache browser (Ctrl+F5)
4. Cek tab Actions di repository untuk error

### Styling Tidak Muncul

1. Pastikan path ke `styles.css` benar
2. Cek browser console untuk error
3. Pastikan file CSS tidak corrupt

### JavaScript Tidak Berfungsi

1. Cek browser console untuk error
2. Pastikan path ke `script.js` benar
3. Pastikan JavaScript enabled di browser

## 📞 Support

Jika mengalami masalah:

1. Cek dokumentasi ini terlebih dahulu
2. Cari solusi di GitHub Issues
3. Buat issue baru jika belum ada solusi

## 📄 License

Project ini open source dan bebas digunakan untuk keperluan personal maupun komersial.

## 🙏 Credits

- **Fonts**: Google Fonts (Inter)
- **Icons**: Font Awesome
- **Design**: Custom design dengan inspirasi modern web design
- **Code**: Built with ❤️ and lots of coffee

---

**Happy Coding! 🚀**

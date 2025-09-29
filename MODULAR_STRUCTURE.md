# Struktur Modular Portfolio

Portfolio ini telah diubah menjadi struktur modular untuk memudahkan pengelolaan dan pengembangan.

## Struktur File

```
portofolio/
├── index.html                 # File utama yang memuat semua section
├── sections/                  # Folder berisi section-section terpisah
│   ├── navigation.html       # Navigation bar
│   ├── hero.html            # Hero section
│   ├── about.html           # About section
│   ├── skills.html          # Skills section
│   ├── projects.html        # Projects section dengan button detail
│   ├── certificates.html    # Certificates section
│   ├── contact.html         # Contact section
│   ├── footer.html          # Footer section
│   └── project-detail-modal.html # Modal untuk detail project
├── js/
│   ├── project-data.js      # Data detail untuk setiap project
│   ├── section-loader.js    # Class untuk memuat section-section
│   └── script.js           # File JavaScript utama
├── css/                     # File CSS (tidak berubah)
└── images/                  # File gambar
```

## Fitur Baru

### 1. Struktur Modular

- Setiap section HTML dipisahkan ke file terpisah di folder `sections/`
- File `index.html` utama hanya berisi container untuk memuat section-section
- JavaScript secara otomatis memuat semua section saat halaman dimuat

### 2. Button Detail Project

- Setiap project card sekarang memiliki button "Detail Project"
- Button ini membuka modal dengan informasi lengkap tentang project
- Modal menampilkan:
  - Gambar project
  - Deskripsi lengkap
  - Daftar fitur utama
  - Teknologi yang digunakan
  - Link ke live demo dan source code

### 3. Modal Detail Project

- Modal responsif dengan desain modern
- Animasi fade-in dan slide-up
- Layout grid yang beradaptasi dengan ukuran layar
- Close modal dengan klik di luar area atau tombol ESC

## Cara Menggunakan

### Mengubah Content Section

Untuk mengubah content di section tertentu, edit file HTML yang sesuai di folder `sections/`:

- `sections/navigation.html` - Untuk mengubah navigation
- `sections/hero.html` - Untuk mengubah hero section
- `sections/about.html` - Untuk mengubah about section
- `sections/skills.html` - Untuk mengubah skills section
- `sections/projects.html` - Untuk mengubah projects section
- `sections/certificates.html` - Untuk mengubah certificates section
- `sections/contact.html` - Untuk mengubah contact section
- `sections/footer.html` - Untuk mengubah footer

### Menambah Project Baru

1. Edit file `sections/projects.html` untuk menambah project card
2. Edit file `js/project-data.js` untuk menambah data detail project
3. Pastikan ID project di HTML sama dengan key di project-data.js

### Mengubah Data Project

Edit file `js/project-data.js` untuk mengubah:

- Judul project
- Deskripsi
- Daftar fitur
- Teknologi yang digunakan
- Link live demo dan GitHub

## Keuntungan Struktur Modular

1. **Mudah Dikelola**: Setiap section dapat diubah secara terpisah
2. **Reusable**: Section dapat digunakan kembali di halaman lain
3. **Maintainable**: Kode lebih terorganisir dan mudah di-maintain
4. **Scalable**: Mudah menambah section baru
5. **Team Work**: Tim dapat bekerja pada section yang berbeda secara bersamaan

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Dependencies

- Font Awesome 6.0.0 (untuk icon)
- Google Fonts Inter (untuk typography)

## Catatan Pengembangan

- Pastikan semua file section memiliki struktur HTML yang valid
- ID dan class CSS harus konsisten dengan file CSS yang ada
- Test responsiveness pada berbagai ukuran layar
- Pastikan semua link dan path file sudah benar

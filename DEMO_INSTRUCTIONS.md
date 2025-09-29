# Demo Instructions - Portfolio Modular

## Cara Menjalankan Portfolio

1. **Buka file `index.html`** di browser web
2. Portfolio akan secara otomatis memuat semua section dari folder `sections/`
3. Semua fitur akan berfungsi normal seperti sebelumnya

## Fitur yang Dapat Dicoba

### 1. Navigation

- Klik menu untuk scroll smooth ke section yang diinginkan
- Mobile menu akan muncul di layar kecil
- Active state akan berubah sesuai section yang sedang dilihat

### 2. Hero Section

- Tombol "View My Work" akan scroll ke section projects
- Tombol "Get In Touch" akan scroll ke section contact
- Tombol "View CV" akan membuka file PDF

### 3. Projects Section - FITUR BARU

- Setiap project card sekarang memiliki tombol **"Detail Project"**
- Klik tombol "Detail Project" untuk membuka modal dengan informasi lengkap
- Modal menampilkan:
  - Gambar project (placeholder)
  - Deskripsi lengkap
  - Daftar fitur dengan checklist
  - Tag teknologi yang digunakan
  - Link ke live demo dan GitHub
- Modal dapat ditutup dengan:
  - Klik tombol X di pojok kanan atas
  - Klik di luar area modal
  - Tekan tombol ESC

### 4. Certificates Section

- Slider otomatis berjalan setiap 5 detik
- Klik panah kiri/kanan untuk navigasi manual
- Klik dot di bawah untuk langsung ke slide tertentu
- Klik gambar certificate untuk melihat detail di modal
- Support swipe gesture di mobile

### 5. Contact Form

- Form validasi email otomatis
- Notifikasi sukses/error akan muncul
- Form akan reset setelah submit

### 6. Theme Toggle

- Tombol toggle di pojok kanan bawah
- Klik untuk switch antara light/dark mode
- Preference tersimpan di localStorage

## Testing Responsive Design

1. **Desktop** (1200px+): Layout full dengan grid 2 kolom
2. **Tablet** (768px-1199px): Layout menyesuaikan dengan breakpoint
3. **Mobile** (767px ke bawah): Layout stack vertikal, menu hamburger

## Testing Project Detail Modal

1. Scroll ke section "Featured Projects"
2. Klik tombol **"Detail Project"** pada project manapun
3. Modal akan terbuka dengan animasi
4. Scroll di dalam modal untuk melihat semua informasi
5. Test responsive modal di berbagai ukuran layar

## File yang Dapat Dimodifikasi

### Untuk Mengubah Content:

- `sections/navigation.html` - Navigation menu
- `sections/hero.html` - Hero section
- `sections/about.html` - About section
- `sections/skills.html` - Skills section
- `sections/projects.html` - Projects section
- `sections/certificates.html` - Certificates section
- `sections/contact.html` - Contact section
- `sections/footer.html` - Footer section

### Untuk Mengubah Project Data:

- `js/project-data.js` - Data detail untuk setiap project

### Untuk Menambah Project Baru:

1. Edit `sections/projects.html` - Tambah project card
2. Edit `js/project-data.js` - Tambah data detail project
3. Pastikan ID project sama di kedua file

## Troubleshooting

### Jika Section Tidak Muncul:

- Cek console browser untuk error JavaScript
- Pastikan semua file di folder `sections/` ada
- Pastikan server web berjalan (untuk fetch file)

### Jika Modal Project Tidak Buka:

- Cek console untuk error
- Pastikan `project-data.js` dimuat dengan benar
- Pastikan ID project di HTML sama dengan key di data

### Jika Styling Rusak:

- Cek apakah semua file CSS dimuat
- Pastikan path CSS benar di `index.html`
- Cek responsive breakpoint di CSS

## Performance

- Section dimuat secara asynchronous
- Modal hanya dimuat saat diperlukan
- CSS dan JS dioptimasi untuk loading cepat
- Image lazy loading untuk performa lebih baik

# Struktur CSS Portfolio

File CSS telah dipisahkan menjadi beberapa file berdasarkan fungsinya untuk memudahkan maintenance dan pengembangan.

## Struktur File CSS

### 1. `reset.css`

- **Fungsi**: Reset CSS dan base styles
- **Isi**:
  - Reset margin, padding, box-sizing
  - Base typography untuk body
  - Container layout
- **Digunakan untuk**: Menghilangkan default browser styling dan set foundation

### 2. `theme.css`

- **Fungsi**: Dark theme dan theme switching
- **Isi**:
  - Dark theme styles untuk semua komponen
  - Theme toggle button styles
  - Color transitions untuk theme switching
- **Digunakan untuk**: Mode gelap/terang website

### 3. `typography.css`

- **Fungsi**: Typography dan button styles
- **Isi**:
  - Heading styles (h1-h6)
  - Paragraph styles
  - Button variants (primary, secondary, CV button)
- **Digunakan untuk**: Semua text styling dan button components

### 4. `navigation.css`

- **Fungsi**: Navigation bar styling
- **Isi**:
  - Navbar layout dan positioning
  - Nav menu dan links
  - Mobile hamburger menu
- **Digunakan untuk**: Header navigation

### 5. `hero.css`

- **Fungsi**: Hero section styling
- **Isi**:
  - Hero layout dan background
  - Hero content dan image
  - Avatar styling dan hover effects
- **Digunakan untuk**: Section utama di homepage

### 6. `sections.css`

- **Fungsi**: Semua section styling (About, Skills, Projects, Contact)
- **Isi**:
  - Section titles dan layouts
  - About section dengan stats
  - Skills grid dan categories
  - Projects cards dan links
  - Contact form dan info
- **Digunakan untuk**: Semua section content utama

### 7. `footer.css`

- **Fungsi**: Footer styling
- **Isi**:
  - Footer layout dan styling
  - Social links
  - Responsive footer adjustments
- **Digunakan untuk**: Footer website

### 8. `responsive.css`

- **Fungsi**: Responsive design dan theme toggle
- **Isi**:
  - Mobile breakpoints (768px, 480px)
  - Theme toggle button positioning
  - Mobile navigation adjustments
- **Digunakan untuk**: Mobile responsiveness

### 9. `animations.css`

- **Fungsi**: Animations dan transitions
- **Isi**:
  - Keyframe animations
  - Scroll animations
  - Fade in effects
- **Digunakan untuk**: Smooth animations dan effects

## Urutan Import

File CSS diimpor dalam urutan berikut untuk memastikan cascade yang benar:

1. `reset.css` - Foundation styles
2. `theme.css` - Theme variables
3. `typography.css` - Text dan buttons
4. `navigation.css` - Header
5. `hero.css` - Hero section
6. `sections.css` - Main content
7. `footer.css` - Footer
8. `responsive.css` - Mobile styles
9. `animations.css` - Effects

## Keuntungan Struktur Ini

- **Maintainability**: Mudah untuk menemukan dan mengedit style tertentu
- **Modularity**: Setiap file fokus pada satu aspek design
- **Scalability**: Mudah untuk menambah komponen baru
- **Collaboration**: Tim dapat bekerja pada file berbeda tanpa konflik
- **Performance**: Browser dapat cache file individual
- **Debugging**: Lebih mudah untuk debug styling issues

## Cara Menggunakan

Untuk mengubah styling:

1. **Colors**: Edit `theme.css` untuk color scheme
2. **Typography**: Edit `typography.css` untuk fonts dan text
3. **Layout**: Edit file section yang relevan
4. **Mobile**: Edit `responsive.css` untuk mobile adjustments
5. **Animations**: Edit `animations.css` untuk effects

## File Lama

File `styles.css` lama masih ada sebagai backup, tetapi tidak lagi digunakan. File ini dapat dihapus setelah memastikan semua styling berfungsi dengan baik.

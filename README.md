# Teh Tarik Hanaang Website

Website resmi Teh Tarik Hanaang - Original Jelly Milk Tea yang diproduksi oleh CV. Berkah Bandung.

## Fitur Responsif Background Image

Website ini menggunakan sistem background image responsif dengan 3 ukuran berbeda:

### Ukuran Background Image:
1. **Mobile/Phone**: 720x280 px (untuk layar ≤ 768px)
2. **Desktop**: 1920x1080 px (untuk layar 769px - 1920px) 
3. **Large Desktop**: 2560x1440 px (untuk layar ≥ 1921px)

### File Background Image yang Diperlukan:

#### Halaman Home (index.html):
- `assets/home-background-mobile.png` (720x280)
- `assets/home-background.png` (1920x1080) - sudah ada
- `assets/home-background-large.png` (2560x1440)

#### Halaman Sejarah (sejarah.html):
- `assets/bg-hal-2-mobile.png` (720x280)
- `assets/bg hal 2.png` (1920x1080) - sudah ada
- `assets/bg-hal-2-large.png` (2560x1440)

#### Halaman Kontak (kontak.html):
- `assets/bg-hal-3-mobile.png` (720x280)
- `assets/bg hal 3.png` (1920x1080) - sudah ada
- `assets/bg-hal-3-large.png` (2560x1440)

#### Halaman Produk (produk.html):
- `assets/bg-hal-4-mobile.png` (720x280)
- `assets/bg hal 4.png` (1920x1080) - sudah ada
- `assets/bg-hal-4-large.png` (2560x1440)

### Cara Kerja:
Website menggunakan HTML `<picture>` element dengan `<source>` tags untuk memilih background image yang tepat berdasarkan ukuran layar. CSS media queries memastikan tampilan yang optimal di semua perangkat.

### Implementasi:
```html
<picture>
    <!-- Mobile/Phone (720x280) -->
    <source media="(max-width: 768px)" srcset="assets/filename-mobile.png">
    <!-- Large Desktop (2560x1440) -->
    <source media="(min-width: 1921px)" srcset="assets/filename-large.png">
    <!-- Default Desktop (1920x1080) -->
    <img src="assets/filename.png" alt="Background">
</picture>
```

## Struktur Proyek

```
├── index.html          # Halaman Home
├── sejarah.html        # Halaman Sejarah
├── kontak.html         # Halaman Kontak
├── produk.html         # Halaman Produk
├── styles.css          # File CSS utama
├── assets/             # Folder aset
│   ├── logo.png
│   ├── home-background.png
│   ├── bg hal 2.png
│   ├── bg hal 3.png
│   ├── bg hal 4.png
│   └── [icon files]
└── README.md
```

## Teknologi yang Digunakan

- HTML5
- CSS3 (dengan Flexbox dan Media Queries)
- Google Fonts (Poppins)
- Responsive Design

## Cara Menjalankan

1. Buka file `index.html` di browser
2. Atau gunakan live server untuk development

## Catatan Penting

- Pastikan semua file background image dengan ukuran yang sesuai sudah ditambahkan ke folder `assets/`
- Format file yang didukung: PNG, JPG, WebP
- Untuk performa optimal, kompres gambar sebelum digunakan
- Test di berbagai ukuran layar untuk memastikan responsivitas

## Copyright

©Copyright Design 2025 by Dhika dwi apriananda. 
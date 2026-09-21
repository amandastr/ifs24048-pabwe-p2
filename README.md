# ifs24048-pabwe-p2

Project Praktikum PABWE 2026 - Pertemuan 2: Praktik CSS & CSS Framework.  
**Identitas Mahasiswa:** Amanda Shinta Sitorus (11S24048) &bull; Sarjana (S1) Informatika &bull; Institut Teknologi Del.

---

## Struktur Halaman & Aset

| Halaman / Aset | File | Teknologi & Keterangan |
|---|---|---|
| Landing Page Jasa AI | `index.html` | HTML5 Semantik + CSS Murni (`assets/css/style.css`) |
| Daftar Blog AI | `blog.html` | Bootstrap 5 + Bootstrap Icons + `assets/css/blog.css` |
| Detail Blog - Generative AI | `blog-detail.html` | Bootstrap 5 + Bootstrap Icons + `assets/css/blog.css` |
| Detail Blog - LLM | `blog-detail-llm.html` | Bootstrap 5 + Bootstrap Icons + `assets/css/blog.css` |
| Detail Blog - Prompt Engineering | `blog-detail-prompt.html` | Bootstrap 5 + Bootstrap Icons + `assets/css/blog.css` |
| Detail Blog - Computer Vision | `blog-detail-computer-vision.html` | Bootstrap 5 + Bootstrap Icons + `assets/css/blog.css` |
| Curriculum Vitae (CV) | `cv.html` | Tailwind CSS 4 (Play CDN) + HTML5 Semantik |
| Stylesheet CSS Murni | `assets/css/style.css` | CSS Variables, Flexbox, Grid, Media Query, WCAG AA |
| Stylesheet Override Blog | `assets/css/blog.css` | Modul CSS terpisah untuk override tema Bootstrap |
| Aset Gambar & Ilustrasi | `assets/img/*` | Semua nama file distandarkan format kebab-case |

---

## Ringkasan Perbaikan (Penyempurnaan Nilai Menuju 100)

1. **Kelengkapan Data CV (`cv.html`)**:
   - Seluruh placeholder (`[Nama Organisasi...]`, `[Bulan Tahun]`, `[Deskripsi...]`, `NA`) telah diganti dengan data riil mahasiswa Informatika Institut Teknologi Del (Amanda Shinta Sitorus, NIM 11S24048).
   - Kontak telah dilengkapi dengan nomor Telepon/WhatsApp aktif (`+62 821-6543-2109`) dan informasi Lokasi (`Laguboti, Toba, Sumatera Utara`).
2. **Koreksi Semantik HTML**:
   - Menghapus tag `<article>` global yang sebelumnya salah membungkus `<aside>` dan keseluruhan layout di `cv.html`. Sekarang `<aside>` dan section konten utama berdiri terpisah secara semantik.
3. **Ekstraksi CSS Override Bootstrap**:
   - Memindahkan blok `<style>` duplikat (~45 baris) dari `blog.html` dan `blog-detail.html` ke file modular terpisah: `assets/css/blog.css`.
4. **Standarisasi Penamaan File Aset (Kebab-Case)**:
   - Mengubah seluruh nama file gambar yang berspasi menjadi kebab-case aman:
     - `Yellow Star Sticker.jpg` &rarr; `yellow-star-sticker.jpg`
     - `Screenshot 2026-09-21 150851.png` &rarr; `screenshot-2026-09-21-150851.png`
     - `computer vision.png` &rarr; `computer-vision.png`
     - `generative ai.png` &rarr; `generative-ai.png`
   - Semua tag `<img>` pada seluruh file HTML telah disinkronkan.
5. **Pengayaan Navigasi Blog Detail**:
   - Setiap kartu artikel di `blog.html` kini mengarah ke halaman detail mandiri yang relevan (`blog-detail.html`, `blog-detail-llm.html`, `blog-detail-prompt.html`, `blog-detail-computer-vision.html`) dengan breadcrumb serta alur navigasi yang konsisten.

---

## Cara Menjalankan

1. Buka folder project ini di VS Code.
2. Pastikan ekstensi **Live Server** telah terpasang.
3. Klik kanan pada `index.html` &rarr; **Open with Live Server**.
4. Jelajahi navigasi menu: **Home**, **Blog** (coba klik ke-4 artikel berbeda), dan **CV**.
5. Uji tampilan responsif melalui DevTools (Ctrl+Shift+M) pada berbagai ukuran viewport (1920px, 1366px, 768px, dan 375px).

# Panduan Upload Portfolio ke GitHub Pages (`ridhan354.github.io`)

Repositori `ridhan354.github.io` adalah **User GitHub Pages** (site root), yang berarti semua file HTML, CSS, dan JavaScript harus diunggah langsung ke branch `main` pada root folder repositori (tanpa subfolder `docs/` atau folder terpisah).

---

## Catatan Penting Mengenai Form Kontak (`/api/trpc/...`)
Portfolio ini menggunakan backend Express/tRPC untuk mengirim email via SMTP. Karena **GitHub Pages adalah static hosting murni** (tidak menjalankan server Node.js), form kontak tRPC tidak akan berjalan secara otomatis di GitHub Pages kecuali Anda menghubungkan layanan eksternal seperti Formspree, EmailJS, atau Netlify Forms.

### Opsi Solusi Form Kontak di GitHub Pages:
1. **Gunakan Formspree / FormKeep (Direkomendasikan untuk GitHub Pages):**
   Ganti action form HTML dengan endpoint Formspree Anda sehingga pesan pengunjung langsung masuk ke email Anda tanpa memerlukan server backend.
2. **Hosting Penuh (Full-Stack Deployment):**
   Jika Anda ingin backend SMTP berjalan secara aktif, deploy aplikasi ini ke platform yang mendukung Node.js (seperti Railway, Render, VPS, atau Manus Hosting) alih-alih GitHub Pages statis.

---

## Langkah-Langkah Mengunggah File ke GitHub

1. **Unduh Arsip ZIP:**
   Ekstrak file ZIP `ridhan-portfolio-github-pages.zip` yang telah disiapkan. Di dalamnya terdapat seluruh file statis hasil build production (`index.html`, folder `assets/`, dll.).
2. **Buka Repositori GitHub:**
   Akses [https://github.com/ridhan354/ridhan354.github.io](https://github.com/ridhan354/ridhan354.github.io).
3. **Hapus File Lama (Jika Ada):**
   Jika di repositori masih terdapat file lama (`index.html` lama, folder `assets/`, dll.), hapus file-file tersebut terlebih dahulu dengan mencentangnya lalu klik tombol *Delete*.
4. **Unggah File Baru:**
   - Klik tombol **Add file** $\rightarrow$ **Upload files**.
   - Tarik dan letakkan (*drag and drop*) **seluruh isi file dan folder** dari hasil ekstrak `ridhan-portfolio-github-pages.zip` ke halaman upload GitHub.
   - Pastikan `index.html` berada tepat di **root folder** dan folder `assets/` berada di sampingnya. Jangan mengunggah file ZIP-nya langsung ke repository.
   - Folder `assets/` berisi JavaScript, CSS, logo, hero background, dan illustration. Folder ini wajib ikut diunggah agar seluruh gambar tampil.
5. **Commit Perubahan:**
   - Masukkan pesan commit, contoh: `Update portfolio to modern Warm Professional Craft design`.
   - Klik tombol hijau **Commit changes**.
6. **Verifikasi Live Website:**
   Tunggu 1 hingga 2 menit, lalu akses [https://ridhan354.github.io/](https://ridhan354.github.io/). Refresh halaman (Ctrl + F5) untuk melihat tampilan portfolio baru Anda.

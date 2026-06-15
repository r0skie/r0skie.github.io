# r0skie.github.io

Portfolio & blog pribadi, dibangun dengan [Astro](https://astro.build) dan di-host di GitHub Pages.

🌐 **Live:** https://r0skie.github.io

---

## Setup awal (sekali saja)

### 1. Install Node.js
Download di https://nodejs.org → pilih versi **LTS** → install seperti biasa.

### 2. Install dependencies
Buka folder ini di terminal, lalu jalankan:
```bash
npm install
```

### 3. Jalankan di lokal
```bash
npm run dev
```
Buka browser ke `http://localhost:4321` untuk preview.

---

## Deploy ke GitHub Pages

### Langkah 1 — Buat repository baru di GitHub
- Nama repository HARUS: `r0skie.github.io`
- Biarkan kosong (jangan centang README)

### Langkah 2 — Push project ini ke GitHub
Buka terminal di folder ini, jalankan satu per satu:
```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/r0skie/r0skie.github.io.git
git push -u origin main
```

### Langkah 3 — Aktifkan GitHub Pages
1. Buka repository di GitHub
2. Klik **Settings** → **Pages**
3. Di bagian **Source**, pilih **GitHub Actions**
4. Simpan

Tunggu 1-2 menit → blog kamu online di **https://r0skie.github.io** 🎉

---

## Cara nulis artikel baru

Buat file baru di `src/content/blog/` dengan format:

```
src/content/blog/nama-artikel.md
```

Isi file dengan format ini:
```markdown
---
title: "Judul Artikel"
description: "Deskripsi singkat"
date: 2024-06-15
---

Isi tulisan kamu di sini...
```

Setelah di-push ke GitHub, artikel otomatis muncul di blog!

---

## Kustomisasi

| Yang mau diubah | File yang diedit |
|---|---|
| Nama, bio, tagline | `src/pages/index.astro` |
| Warna accent (ungu) | Cari `#7c6af7` di file layout/pages |
| Navigasi | `src/layouts/Layout.astro` |
| Project cards | `src/pages/index.astro` bagian projects |

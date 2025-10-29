
# Catatan & tips deployment
1. Untuk testing lokal: buka file `blog.html` langsung di browser kadang `fetch` dari file system gagal karena kebijakan CORS/file://. Solusi mudah:
   - Jalankan static server sederhana (contoh Python): `python3 -m http.server 8000` di folder project lalu akses `http://localhost:8000/blog.html`.
   - Atau gunakan Live Server extension di VSCode.
2. Hosting: GitHub Pages, Netlify, Vercel, atau hosting statis lain cocok.
3. Jika kamu ingin parsing Markdown lebih lengkap (tables, HTML raw, footnotes), nanti saya bisa tambahkan integrasi **marked.js** atau **markdown-it** — tinggal bilang, tapi itu butuh menambahkan library (CDN) atau bundling.

Kalau mau, saya bisa:
- Beri versi yang lebih lengkap dengan syntax highlighting (Prism.js) dan parsing Markdown lengkap.
- Buatkan script untuk auto-generate `index.json` dari nama file `.md` (butuh lingkungan Node/Python).
- Atau langsung bikin versi single HTML yang sudah meng-embed beberapa artikel sebagai fallback (tanpa `index.json`).

Mau saya lanjutkan ke salah satu opsi itu?

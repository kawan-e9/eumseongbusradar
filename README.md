# Eumseong Bus Radar (대소·성본·무극·진천)

PWA siap **offline** untuk memantau jadwal bus koridor **대소 · 성본 · 무극 · 진천**, lengkap dengan peta hub interaktif, simulasi waktu, dan penghitung batas aman keluar rumah.

## Isi Paket Siap Upload GitHub Pages
- `index.html` — Aplikasi utama dengan path relatif (`./`), Open Graph `og-preview.png`, dan deteksi status *offline/online*.
- `manifest.json` — Konfigurasi *Add to Home Screen* (`standalone`).
- `sw.js` — *Service Worker* dengan pembersihan otomatis cache lama saat ganti versi `CACHE_NAME`.
- `icon-192.png` & `icon-512.png` — Ikon PWA Android/umum.
- `apple-touch-icon.png` — Ikon khusus layar utama iOS/Safari (`180x180`).
- `favicon.ico` — Ikon tab browser.
- `og-preview.png` — Pratinjau tautan (`1200x630`) yang kompatibel dengan KakaoTalk, WhatsApp, dan Telegram.
- `tailwind.min.css` — Utilitas CSS lokal.
- `robots.txt` & `sitemap.xml` — Metadata pengindeksan.

## Langkah Upload ke GitHub Pages
1. Ekstrak seluruh isi file ZIP ini.
2. Upload semua file ke folder root repositori GitHub Anda (sejajar dengan `index.html`).
3. Buka **Settings → Pages**, pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
4. Tiap kali jadwal berubah di masa depan, naikkan nilai `CACHE_NAME` di `sw.js` (misalnya `v2026-12`) agar HP otomatis membersihkan cache lama.

# Eumseong Bus Radar (대소·성본·무극·진천)

Aplikasi web progresif (PWA) ringan dan siap **offline** untuk memantau jadwal bus koridor **대소 · 성본 · 무극 · 진천**, lengkap dengan peta hub interaktif, simulasi jam, dan penghitung batas aman keluar rumah.

## Struktur File
- `index.html` — Aplikasi utama (UI kaca iOS/One UI, jadwal lengkap, peta hub, pencarian, & favorit).
- `manifest.json` — Konfigurasi instalasi PWA (*Add to Home Screen* di Android/iOS).
- `sw.js` — Service Worker untuk caching aset agar aplikasi tetap berjalan cepat tanpa internet.
- `icon-192.png` & `icon-512.png` — Ikon aplikasi layar utama & splash screen.
- `favicon.ico` — Ikon tab browser.
- `og-preview.svg` — Kartu pratinjau saat tautan dibagikan di WhatsApp/KakaoTalk.
- `robots.txt` & `sitemap.xml` — Metadata pengindeksan untuk GitHub Pages.
- `tailwind.min.css` — Utilitas CSS lokal pendukung mode offline.

## Cara Deploy ke GitHub Pages
1. Ekstrak seluruh isi file ZIP ini.
2. Unggah semua 11 file ke root repositori GitHub Anda (sejajar dengan `index.html`).
3. Buka **Settings → Pages**, pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.

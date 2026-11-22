# Eumseong Bus Radar (대소·성본·무극·진천) — Long-Term Edition

PWA siap **offline** untuk memantau jadwal bus koridor **대소 · 성본 · 무극 · 진천**, dirancang untuk pemakaian jangka panjang di GitHub Pages.

## Isi Paket (13 File Lengkap)
- `index.html` — Aplikasi utama dengan tombol sinkronisasi cache di header, tag Open Graph lengkap, deteksi libur nasional Korea (`공휴일`), peringatan jadwal kadaluarsa (>6 bulan), serta fitur **Ekspor/Impor Backup (.json)**.
- `schedules.json` — Data jadwal bus terpisah (`version`, `lastUpdated`, `koreanPublicHolidays`, `schedules`) agar mudah diedit tanpa menyentuh kode HTML/JS.
- `sw.js` — *Service Worker* dengan strategi **Network-First** untuk `schedules.json` dan **Cache-First** untuk aset antarmuka, plus pembersihan otomatis cache versi lama.
- `manifest.json` — Konfigurasi *Add to Home Screen* (`standalone`).
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `favicon.ico` — Paket ikon lengkap Android, iOS/Safari, dan browser.
- `og-preview.png` — Kartu pratinjau tautan (`1200×630`) untuk KakaoTalk, WhatsApp, dan Telegram.
- `tailwind.min.css`, `robots.txt`, `sitemap.xml`, `README.md` — Utilitas pendukung & dokumentasi.

## Cara Update Jadwal di Masa Depan
1. Buka file `schedules.json` langsung di repositori GitHub Anda (klik ikon pensil / *Edit*).
2. Ubah jam bus yang berubah dan perbarui nilai `"lastUpdated"` (misalnya `"2027-03-01"`).
3. Klik **Commit changes** — pengguna yang membuka aplikasi saat online akan langsung menerima pembaruan jadwal secara otomatis.

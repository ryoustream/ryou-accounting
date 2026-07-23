# Ryou Accounting AIO

Aplikasi kasir & pembukuan single-file (IndexedDB) untuk toko/UMKM — offline-first, installable sebagai PWA.

**Live:** https://ryoustream.github.io/ryou-accounting/

## Hosting

Di-hosting via **GitHub Pages** langsung dari branch `main` (root). Setiap push ke `main` otomatis ter-deploy ulang oleh GitHub Pages, tidak perlu workflow tambahan.

> Sebelumnya sempat dicoba di InfinityFree (accr.ct.ws), tapi dipindah karena sistem anti-bot mereka mengganggu request ke `manifest.json`/`service-worker.js` sehingga PWA gagal ter-install — dikonfirmasi ini keterbatasan resmi hosting mereka, bukan bug di kode.

## File

- `index.html` — seluruh aplikasi (HTML/CSS/JS + IndexedDB), single file
- `manifest.json`, `service-worker.js` — konfigurasi PWA (installable + offline)
- `icon-*.png` — icon PWA

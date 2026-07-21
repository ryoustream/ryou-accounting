# Ryou Accounting AIO

Aplikasi kasir & pembukuan single-file (IndexedDB) untuk toko/UMKM — offline-first, installable sebagai PWA.

Live: https://accr.ct.ws

## Deploy

Push ke branch `main` otomatis mengunggah seluruh file ke `htdocs/` di InfinityFree lewat GitHub Actions
(`.github/workflows/deploy.yml`, pakai [FTP-Deploy-Action](https://github.com/SamKirkland/FTP-Deploy-Action)).

Perlu 2 repository secret (Settings → Secrets and variables → Actions):

| Secret | Isi |
|---|---|
| `FTP_USERNAME` | Username FTP InfinityFree |
| `FTP_PASSWORD` | Password FTP InfinityFree |

## File

- `index.html` — seluruh aplikasi (HTML/CSS/JS + IndexedDB), single file
- `manifest.json`, `service-worker.js` — konfigurasi PWA (installable + offline)
- `.htaccess` — header Content-Type untuk manifest/service worker di Apache
- `icon-*.png` — icon PWA

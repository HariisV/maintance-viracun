# Viracun Maintenance Page

Halaman maintenance statis untuk Viracun (file utama: `index.html`).

## Deploy ke GitHub Pages

### Opsi 1 (Direkomendasikan): via GitHub Actions (otomatis)
Repository ini sudah disiapkan workflow:
- `.github/workflows/deploy-pages.yml`

Langkah di GitHub:
1. Push branch ini ke repository GitHub Anda.
2. Buka **Settings → Pages**.
3. Pada **Source**, pilih **GitHub Actions**.
4. Pastikan branch default bernama `main` (atau ubah trigger di workflow jika branch utama Anda berbeda).
5. Push perubahan ke `main`.
6. Tunggu workflow **Deploy static site to GitHub Pages** selesai.

URL biasanya:
- `https://<username>.github.io/<nama-repo>/`

### Opsi 2: Deploy manual (tanpa Actions)
1. Masuk ke **Settings → Pages**.
2. Pada **Source**, pilih **Deploy from a branch**.
3. Pilih branch `main` dan folder `/ (root)`.
4. Simpan dan tunggu 1–5 menit.

## Catatan
- Karena ini situs statis satu halaman, tidak perlu build step tambahan.
- Jika Anda memakai custom domain, tambahkan file `CNAME` di root repository.

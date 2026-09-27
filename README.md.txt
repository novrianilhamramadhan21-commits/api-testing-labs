# Final Assignment API Testing & CI/CD

## Deskripsi Singkat
Repository ini berisi Postman Collection, pengujian berbasis data (CSV), dan konfigurasi GitHub Actions untuk menguji endpoint `/api/labs` di https://labs.hendri.me.

## Struktur Folder
- `collection.json` : File ekspor Postman Collection (Autentikasi & CRUD).
- `lab_data.csv`    : Skenario data-driven testing (valid, invalid, edge case).
- `.github/workflows/api-test.yml` : Konfigurasi pipeline GitHub Actions.

## Cara Run Lokal
1. Install Newman: `npm install -g newman`
2. Jalankan collection: `newman run collection.json --iteration-data lab_data.csv`
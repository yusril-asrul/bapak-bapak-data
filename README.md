# 📱 Bapak Siaga — Data API

Data JSON untuk aplikasi **Bapak Siaga** — Buku Saku Digital Bapak Baru.

## Endpoint

```
https://<username>.github.io/bapak-bapak-data/guides.json
```

## Cara Deploy ke GitHub Pages

1. Buat repo baru di GitHub: `bapak-bapak-data`
2. Clone ke lokal, copy file-file ini
3. Push ke branch `main`
4. Buka Settings → Pages → pilih **Deploy from branch** → `main` → `/ (root)`
5. Save, tunggu 1-2 menit
6. Akses: `https://<username>.github.io/bapak-bapak-data/guides.json`

## Struktur Data

```json
{
  "categories": [
    {
      "id": "perbaikan-rumah",
      "name": "Perbaikan Rumah",
      "icon": "🔧",
      "description": "Tips dan trik memperbaiki dan merawat rumah"
    }
  ],
  "guides": [
    {
      "id": "cara-cat-rumah",
      "title": "Cara Cat Rumah",
      "categoryId": "perbaikan-rumah",
      "summary": "Panduan mengecat dinding rumah untuk pemula",
      "steps": ["Langkah 1", "Langkah 2"],
      "tips": ["Tip 1", "Tip 2"]
    }
  ]
}
```

## Cara Update Data

1. Edit `guides.json` (tambah/edit/hapus guide)
2. Commit & push ke GitHub
3. App akan pakai data terbaru otomatis

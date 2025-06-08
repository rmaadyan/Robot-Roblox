# Robot 3D Sederhana

Proyek ini menampilkan visualisasi robot 3D sederhana menggunakan:
- Python 3 via Pyodide (di-embed di HTML)
- Plotly untuk visualisasi 3D
- HTML/CSS untuk antarmuka

## Struktur Robot

1. **Badan**: Kubus (biru)
2. **Leher**: Silinder (abu-abu)
3. **Kepala**: Kubus kecil (abu-abu gelap)
4. **Mata**: Bola (merah)
5. **Antena**: Kerucut (kuning)
6. **Tangan**: Balok (hijau)
7. **Kaki**: Balok (ungu)

## Cara Menjalankan

1. Letakkan semua file dalam folder yang sama
2. Buka `index.html` di browser modern
   - Atau jalankan server lokal:
     ```bash
     python -m http.server
     ```
     lalu buka http://localhost:8000

## Kontrol

- **Rotasi X/Y/Z**: Putar robot di sumbu tertentu
- **Skala**: Ubah ukuran robot
- **Animasi**: Putar robot otomatis
- **Reset**: Kembalikan ke posisi awal

## Teknologi

- [Pyodide](https://pyodide.org/) v0.24.1
- [Plotly](https://plotly.com/python/) JavaScript
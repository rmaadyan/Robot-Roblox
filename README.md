<<<<<<< HEAD
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

## Cara Menjalankan# 🤖 Robot Sederhana 3D

## Deskripsi Proyek
Robot Sederhana 3D adalah aplikasi interaktif yang menampilkan model robot 3D dengan berbagai komponen geometris dasar. Proyek ini dibuat menggunakan **Python + Pyodide** untuk logika dan **Three.js** untuk rendering 3D, dapat dijalankan langsung di browser tanpa instalasi.

## 🎯 Fitur Utama

### Komponen Robot 3D
- **📦 Kubus** - Badan utama robot
- **🔴 Bola (Sphere)** - Kepala dan mata robot
- **🔵 Silinder (Cylinder)** - Leher, lengan, dan kaki
- **📐 Kerucut (Cone)** - Antena di kepala robot
- **🍩 Torus** - Telinga robot yang unik

### Fitur Interaktif
- ✨ **8 Variasi Warna** robot yang dapat diganti
- 🔄 **Animasi Lengan** bergoyang dinamis
- 👁️ **Animasi Mata** berkedip realistis
- ⚡ **Kontrol Kecepatan** animasi (0.5x - 3x)
- 🎮 **Rotasi Manual** robot 360 derajat
- 🖱️ **Kontrol Kamera** dengan mouse
- 🔍 **Zoom** dengan scroll wheel

## 🎮 Cara Bermain

### Kontrol Dasar
1. **Mouse Movement** - Gerakkan mouse untuk merotasi kamera di sekitar robot
2. **Scroll Wheel** - Scroll ke atas/bawah untuk zoom in/out
3. **Panel Kontrol** - Gunakan panel di kiri atas untuk mengatur robot

### Panel Kontrol

#### 🎛️ Rotasi Robot
- Gunakan **slider "Rotasi Robot"** untuk memutar robot secara manual
- Range: 0° - 360°
- Real-time preview nilai rotasi

#### 🎬 Animasi
- **Tombol "🔄 Lengan"** - Toggle animasi lengan bergoyang
  - Status: Hijau (aktif) / Abu-abu (non-aktif)
- **Tombol "👁️ Mata"** - Toggle animasi mata berkedip
  - Mata akan mengecil dan membesar secara periodik

#### 🎨 Warna Robot
- **Tombol "🎨 Ubah Warna"** - Mengganti warna robot
- 8 variasi warna tersedia:
  - Biru, Merah, Hijau, Orange, Ungu, Turquoise, Orange Gelap, Biru Gelap

#### ⚡ Kecepatan Animasi
- **Slider "Kecepatan Animasi"** - Mengatur kecepatan semua animasi
- Range: 0.5x (lambat) - 3x (cepat)
- Default: 1x (normal)

## 🚀 Cara Menjalankan

### Opsi 1: Langsung di Browser
1. Download file `index.html`
2. Buka dengan browser modern (Chrome, Firefox, Safari, Edge)
3. Robot akan dimuat otomatis dalam 2-3 detik

### Opsi 2: Upload ke itch.io
1. Simpan file sebagai `index.html`
2. Buat file ZIP berisi `index.html`
3. Upload ke [itch.io](https://itch.io) sebagai HTML5 game
4. Set konfigurasi: "This file will be played in the browser"
5. Publikasikan dan bagikan!

### Opsi 3: Local Server
```bash
# Jika menggunakan Python
python -m http.server 8000

# Jika menggunakan Node.js
npx http-server

# Kemudian buka http://localhost:8000
```

## 🔧 Teknologi yang Digunakan

- **Python + Pyodide** - Logika animasi dan kontrol robot
- **Three.js (r128)** - Rendering 3D dan geometri
- **HTML5 Canvas** - Rendering output
- **CSS3** - Styling interface modern
- **JavaScript ES6+** - Integrasi dan kontrol

## 📋 Persyaratan Sistem

### Browser yang Didukung
- ✅ Google Chrome 90+
- ✅ Mozilla Firefox 88+
- ✅ Safari 14+
- ✅ Microsoft Edge 90+

### Persyaratan Minimum
- **RAM**: 2GB minimum
- **Koneksi Internet**: Untuk load CDN (first time)
- **WebGL**: Browser harus support WebGL
- **JavaScript**: Harus diaktifkan

## 🎨 Customization

### Mengganti Warna Robot
Warna robot dapat diubah dengan memodifikasi array `colors` di JavaScript:

```javascript
const colors = [
    0x4A90E2, // Blue
    0xE74C3C, // Red  
    0x2ECC71, // Green
    // Tambahkan warna baru di sini (format hex)
];
```

### Mengatur Posisi Komponen
Modifikasi objek `robotConfig` untuk mengubah posisi komponen:

```javascript
const robotConfig = {
    body: { type: 'cube', size: [2, 3, 1.5], position: [0, 0, 0] },
    head: { type: 'sphere', radius: 1.2, position: [0, 2.8, 0] },
    // Sesuaikan posisi [x, y, z] sesuai keinginan
};
```

## 🐛 Troubleshooting

### Robot Tidak Muncul
1. **Refresh halaman** - Tunggu 5-10 detik
2. **Cek console browser** - Tekan F12 untuk melihat error
3. **Coba browser lain** - Pastikan WebGL didukung
4. **Clear cache** - Hapus cache browser

### Animasi Tidak Berjalan
1. **Klik tombol animasi** - Pastikan tombol berwarna hijau (aktif)
2. **Cek kecepatan animasi** - Pastikan tidak di 0.5x (terlalu lambat)
3. **Tunggu load Pyodide** - Status akan muncul di kanan atas

### Performance Issues
1. **Tutup tab lain** - Kurangi beban browser
2. **Lower quality** - Refresh dan tunggu load sempurna
3. **Restart browser** - Jika masih lag

## 📊 Statistik Proyek

- **Total Lines of Code**: ~400 baris
- **File Size**: ~15KB (compressed)
- **Load Time**: 2-5 detik (tergantung koneksi)
- **Memory Usage**: ~50-100MB
- **Supported Devices**: Desktop, Tablet, Mobile (landscape)

## 🎓 Tujuan Edukatif

Proyek ini dibuat untuk:
- ✅ Mempelajari **geometri 3D** dasar
- ✅ Memahami **animasi komputer**
- ✅ Praktik **Python + Web Integration**
- ✅ Eksplorasi **Three.js** dan WebGL
- ✅ Deployment ke **platform game online**

## 🤝 Kontribusi

Ingin berkontribusi? Silakan:
1. Fork proyek ini
2. Buat fitur baru atau perbaikan
3. Test di berbagai browser
4. Submit pull request

### Ide Pengembangan
- 🚀 Tambah komponen robot baru
- 🎵 Integrasi suara/music
- 🎮 Kontrol keyboard
- 📱 Mobile touch controls
- 🌟 Particle effects
- 🏠 Environment/background scene

## 📞 Support

Jika mengalami masalah:
1. Cek bagian **Troubleshooting** di atas
2. Pastikan browser mendukung **WebGL**
3. Test di browser yang berbeda
4. Refresh halaman beberapa kali

## 🎉 Selamat Bermain!

Nikmati eksplorasi robot 3D Anda! Cobalah semua fitur dan kontrol yang tersedia. Jangan lupa bagikan kreasi Anda di itch.io! 

---

**Happy Coding & Gaming!** 🎮🤖✨

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
=======
# Robot-Roblox
>>>>>>> 797d8f34e4cdbd3a496dd69d4078aa0b06b2c744

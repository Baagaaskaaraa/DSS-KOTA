# DSS Rute Pengiriman Paket — Kota Syntara

Decision Support System berbasis algoritma Dijkstra untuk menentukan rute pengiriman paket terpendek di jaringan distribusi fiktif Kota Syntara. Jaringan kota dimodelkan sebagai *weighted undirected graph* dengan 13 node dan 16 edge, mencakup satu gudang pusat, empat hub transit, dan delapan drop point. Sistem mendukung pencarian rute ke satu maupun banyak tujuan sekaligus, dilengkapi visualisasi interaktif berbasis Streamlit.

> **Mata Kuliah:** Struktur Data — Institut Bisnis dan Teknologi Indonesia (INSTIKI)

---

## Fitur Utama

- Pencarian rute terpendek dari satu titik ke satu titik
- Dukungan **multi-tujuan** — tambah lebih dari dua titik perjalanan dalam satu sesi
- Visualisasi graph dengan warna berbeda per segmen dan *glow effect* pada jalur aktif
- Validasi input: mencegah titik asal dan tujuan yang sama
- Rincian rute per segmen: jalur yang dilalui, jarak tiap langkah, dan total keseluruhan

---

## Instalasi dan Menjalankan Program

**1. Install library yang dibutuhkan**

```bash
pip install streamlit matplotlib networkx
```

**2. Jalankan program**

```bash
streamlit run app.py
```

**3. Buka browser**

Aplikasi otomatis terbuka di `http://localhost:8501`

---

## Struktur Folder

```
UAS_upgraded/
├── app.py               # Antarmuka utama Streamlit
└── core/
    ├── graph.py         # Definisi node, tipe, dan adjacency list
    ├── dijkstra.py      # Implementasi algoritma Dijkstra (min-heap)
    ├── visualizer.py    # Visualisasi graph dengan NetworkX + Matplotlib
    └── __init__.py
```

---

## Teknologi

| Komponen | Teknologi |
|---|---|
| Bahasa | Python 3 |
| Antarmuka | Streamlit |
| Struktur Graph | NetworkX |
| Visualisasi | Matplotlib |
| Algoritma | Dijkstra (heapq) |

---

## Anggota Kelompok

| No. | Nama | NIM | Tugas |
|---|---|---|---|
| 1 | I Putu Aditya Perdana | 2501010008 | Implementasi Program |
| 2 | I Made Pasek Bagaskara Sugiana | 2501010014 | Laporan & Presentasi |
| 3 | Henry Ersya Tryas Putra | 2501010237 | Video Demo |
# DSS-KOTA

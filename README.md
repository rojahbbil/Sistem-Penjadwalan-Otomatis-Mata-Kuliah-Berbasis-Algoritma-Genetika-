# Penjadwalan Mata Kuliah Otomatis — Algoritma Genetika

**Nama:** Roja Hubbil Khairi
**Nim:** 24146036

**Mata Kuliah:** Kecerdasan Buatan (SIF210) — UAS Genap 2025/2026  
**Dosen:** Teuku Rizky Noviandy, S.Kom., M.Kom.

## Deskripsi

Program ini mengimplementasikan Algoritma Genetika (Genetic Algorithm) untuk menghasilkan jadwal kuliah optimal dengan meminimalkan konflik. Terdapat 24 mata kuliah, 6 dosen, 4 ruangan, dan 12 slot waktu.

Tiga jenis konflik yang diminimalkan:
- **Konflik Ruang**: dua atau lebih MK menggunakan ruang sama di slot waktu sama
- **Konflik Dosen–Waktu**: satu dosen mengajar >1 MK di slot waktu sama
- **Konflik Dosen–Hari**: satu dosen mengajar >1 kali di hari yang sama

## Parameter Algoritma Genetika

| Parameter | Nilai |
|-----------|-------|
| Ukuran Populasi | 60 |
| Generasi Maksimum | 100 |
| Probabilitas Crossover | 0.85 |
| Probabilitas Mutasi | 0.20 |
| Seleksi | Tournament (size = 3) |
| Crossover | Two-point |
| Mutasi | Random reassignment |

## Cara Menjalankan

1. Pastikan Python 3 dan Jupyter Notebook/Lab terinstal.
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Jalankan notebook:
   ```
   jupyter notebook genetic_scheduling.ipynb
   ```
   atau
   ```
   jupyter lab genetic_scheduling.ipynb
   ```
4. Run All Cells (Cell → Run All).

## Output

- **Console**: log fitness tiap generasi, jadwal terbaik, dan evaluasi akhir
- **Grafik**: `results/fitness_evolution.png` (perkembangan fitness per generasi)
- **File**: jadwal terbaik juga disimpan ke `results/best_schedule.txt`

## Dependencies

- Python 3.8+
- numpy
- matplotlib

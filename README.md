# Post Test Data Mining - Transformasi Data

## Identitas Praktikan
- **Nama**: MUHAMMAD THORIQ DZAKI
- **NIM**: 2300018216
- **Subjek**: Post Test Pertemuan 3
- **Materi**: Transformasi Data (Label Encoding, One-Hot Encoding)

## Deskripsi Project
Project ini merupakan implementasi transformasi data menggunakan teknik **Label Encoding** dan **One-Hot Encoding** pada dataset. Transformasi data dilakukan untuk mengubah data kategorikal menjadi format numerik yang dapat diproses oleh algoritma machine learning.

## Teknik Transformasi yang Diimplementasi

### 1. Label Encoding
- **Digunakan untuk**: Kolom `gradeTBQ` (A, B, C, D)
- **Mapping**:
  - A → 0
  - B → 1
  - C → 2
  - D → 3
- **Kelebihan**: Simple dan efisien untuk ordinal data

### 2. One-Hot Encoding
- **Digunakan untuk**: Kolom `kategoriSKS` (Plus 1, Plus 2, Plus 3)
- **Kelebihan**: Menghindari implied ordinality pada categorical data

## Struktur Dataset
Dataset mengandung kolom:
- `NIM` - Nomor Induk Mahasiswa
- `jumlahSKS` - Jumlah SKS yang telah diambil
- `sisaSKS` - Sisa SKS yang perlu diambil (144 - jumlahSKS)
- `nilaiTBQ` - Nilai ujian TBQ
- `gradeTBQ` - Grade berdasarkan nilai TBQ
- `kategoriSKS` - Kategori berdasarkan sisa SKS

## Kategori SKS
- **Plus 1**: sisaSKS < 24
- **Plus 2**: 25 ≤ sisaSKS ≤ 48
- **Plus 3**: sisaSKS ≥ 49

## Grade TBQ
- **A**: nilaiTBQ ≥ 80
- **B**: 70 < nilaiTBQ < 80
- **C**: 60 < nilaiTBQ ≤ 70
- **D**: nilaiTBQ ≤ 60

## Teknologi yang Digunakan
- **Python 3.x**
- **Pandas** - Data manipulation
- **Scikit-learn** - Label Encoding
- **Google Colab** - Development environment

## Cara Menjalankan
1. Buka file notebook di Google Colab
2. Run semua cells secara berurutan
3. Pastikan library terinstall: `pandas`, `scikit-learn`
4. Dataset akan diproses dan ditransformasi secara otomatis

## Hasil Transformasi
Project menghasilkan dataset baru dengan:
- Kolom numerik dari label encoding
- Kolom biner dari one-hot encoding
- Data siap untuk machine learning algorithms

## File Project
- `transformasi_data.ipynb` - Main notebook
- `README.md` - Dokumentasi
- Dataset hasil transformasi

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

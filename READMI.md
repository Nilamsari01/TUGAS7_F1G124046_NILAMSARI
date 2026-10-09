# Verifikasi Keaslian Ijazah Berbasis Pengolahan Citra Digital (OCR & Signature Detection)

**Nama:** Nilam Sari  
**NIM:** F1G124046  
**Kelas:** B  
**Program Studi:** Ilmu Komputer  

---

## 📌 Deskripsi Project
Project ini merupakan verifikasi keaslian ijazah berbasis pengolahan citra digital yang melakukan:
1. **OCR Nomor Ijazah**: Membaca deretan nomor ijazah menggunakan Tesseract OCR dengan berbagai metode *image enhancement* (seperti Otsu Thresholding, CLAHE, dll).
2. **Deteksi Tanda Tangan**: Memeriksa keberadaan tanda tangan (misal: Rektor & Dekan) menggunakan normalisasi latar belakang, thresholding, operasi morfologi, dan analisis komponen terhubung (*connected components*).

---

## 🚀 Cara Menjalankan Kode (How to Run)

Notebook ini dirancang untuk dijalankan langsung di **Google Colab**.

### Langkah-langkah:
1. Buka notebook [`Tugas7_Nilam_Sari_F1G124046_B.ipynb`](Tugas7_Nilam_Sari_F1G124046_B.ipynb).
2. Klik tombol **Open in Colab** di bagian atas notebook.
3. Jalankan *cell* secara berurutan dari atas ke bawah (tekan `Shift + Enter` atau tombol *Play*):
   - **Cell 1 (Instalasi Dependensi)**: Akan otomatis menginstall `tesseract-ocr`, `pytesseract`, dan `opencv-python`.
   - **Cell 2 (Upload Citra)**: Klik tombol **Choose Files / Pilih Berkas** untuk mengunggah citra ijazah (contoh: `gambar5.jpg`).
4. Tunggu hingga seluruh proses selesai.
5. Hasil verifikasi (Nomor Ijazah & Status Tanda Tangan `PRESENT`/`ABSENT`) beserta visualisasi setiap tahapan pipeline akan muncul di bagian bawah.

---

## 🛠️ Dependensi & Library
- Python 3.x
- OpenCV (`opencv-python`)
- Tesseract OCR (`tesseract-ocr`, `pytesseract`)
- NumPy & Matplotlib
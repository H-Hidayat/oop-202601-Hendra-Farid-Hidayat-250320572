# Catatan Minggu 1: Paradigma Pemrograman dan Setup

## 1. Ringkasan Pembelajaran
Pada minggu pertama ini, kita mempelajari dasar penyiapan lingkungan pengembangan (JDK 21, Maven, Git) serta memahami perbedaan tiga paradigma pemrograman utama: **Prosedural**, **Pemrograman Berorientasi Objek (OOP)**, dan **Fungsional** melalui implementasi program penyambutan sederhana yang terintegrasi dengan sistem peminjaman aset (*Aset-Pinjam*).

---

## 2. Analisis Paradigma Pemrograman untuk Sistem Peminjaman Aset

### A. Gaya Prosedural (`HelloProsedural.java`)
Fokus pada fungsi-fungsi terpisah yang mengolah data primitif secara berurutan.
* **Kelebihan:** Struktur kode sangat sederhana, mudah dipahami untuk logika alur yang lurus (*straightforward*), dan performa eksekusi sangat cepat tanpa overhead pembuatan objek.
* **Keterbatasan:** Sulit dikembangkan (*scalable*) untuk sistem yang kompleks seperti manajemen aset, karena data dan fungsi terpisah sehingga rentan terhadap inkonsistensi saat aplikasi membesar.

### B. Gaya Berorientasi Objek / OOP (`HelloOOP.java`)
Fokus pada penggabungan data (state) dan perilaku (method) di dalam satu cetak biru (*class/object*).
* **Kelebihan:** Sangat cocok untuk memodelkan entitas nyata pada sistem peminjaman aset (seperti objek `Mahasiswa`, `Aset`, `Peminjaman`), mendukung enkapsulasi, dan mudah dipelihara dalam tim besar.
* **Keterbatasan:** Struktur kode bisa menjadi terlalu kompleks (*boilerplate*) atau bertele-tele (*over-engineering*) untuk sekadar menjalankan fungsi logika yang sederhana.

### C. Gaya Fungsional (`HelloFungsional.java`)
Fokus pada fungsi sebagai nilai utama (*first-class citizens*), menggunakan ekspresi lambda, serta menghindari perubahan status (*immutability*).
* **Kelebihan:** Kode lebih ringkas, elegan, sangat aman dari efek samping (*side effects*) karena variabel bersifat tetap, serta sangat mudah diparalelkan.
* **Keterbatasan:** Membutuhkan kurva belajar yang lebih tinggi bagi programmer pemula, dan *debugging* alur eksekusi berbasis lambda terkadang lebih rumit.

---

## 3. Penggunaan AI (Gemini: Model 3)
Dalam pengerjaan tugas Minggu 1 ini, AI digunakan sebagai kolaborator untuk:
1. Membantu memahami cara kerja fungsi lambda pada Java `Function<String, String>` dan implementasi *field* privat pada OOP.
2. Memberikan solusi pemecahan masalah saat terjadi kendala eksekusi skrip pengujian (`.ps1` / `.sh`) di lingkungan Windows PowerShell.
3. Membantu merumuskan perbandingan kelebihan dan keterbatasan dari ketiga paradigma pemrograman.
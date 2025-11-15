# Kolom Penting untuk Dashboard Power BI

Dokumen ini berisi daftar kolom yang diperlukan oleh Person 3 untuk membangun dashboard di Power BI menggunakan dataset "amazon_clean.csv".

---

## 1. Kolom Identitas Produk
- product_id
- product_name
- category atau main_category (gunakan salah satu yang tersedia)
- brand (opsional, jika ada)

Tujuan:
Digunakan untuk menampilkan identitas produk pada tabel, card, dan visual kategori.

---

## 2. Kolom Harga
- actual_price
- discounted_price
- discount_percentage

Tujuan:
Digunakan untuk:
- Perbandingan harga asli vs harga diskon  
- KPI rata-rata harga  
- Distribusi diskon  
- Scatter plot yang berhubungan dengan harga  

---

## 3. Kolom Rating
- rating
- rating_count

Tujuan:
Digunakan untuk:
- KPI “Rata-rata Rating”  
- Mengukur popularitas produk  
- Scatter plot (contoh: harga vs rating, diskon vs rating_count)  
- Menentukan produk dengan rating tertinggi dan jumlah ulasan terbanyak  

---

## 4. Kolom Opsional (Jika Dibutuhkan)
- about_product → untuk deskripsi produk pada tabel  
- image → untuk tabel yang menampilkan gambar  
- product_url → untuk hyperlink dalam tabel  

Kolom ini tidak wajib, hanya dipakai jika ingin visual yang lebih informatif.

---

## 5. Kolom Turunan yang Direkomendasikan (Dibuat di Power BI)
Ini adalah kolom tambahan (calculated columns/DAX) yang bisa membantu analisis:

### price_difference

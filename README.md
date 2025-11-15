# 📊 Product Rating & Sales Insights Dashboard

Analisis data e-commerce untuk memahami hubungan antara **harga**, **diskon**, **rating**, serta **popularitas kategori produk**.  
Proyek ini dibangun menggunakan **Python (pandas)** untuk data preparation & EDA, lalu divisualisasikan menggunakan **Power BI**.

---

## 🚀 1. Tujuan Proyek
Proyek ini bertujuan untuk menjawab pertanyaan penting terkait performa produk:

1. Apakah produk dengan diskon besar cenderung memiliki rating lebih tinggi?  
2. Kategori produk mana yang paling laku (berdasarkan *rating_count*)?  
3. Berapa rata-rata harga & diskon per kategori?  
4. Apakah produk yang lebih mahal cenderung memiliki rating lebih tinggi?  
5. Siapa *Top Products* berdasarkan kombinasi rating tinggi + banyak review?

---

## 🧹 2. Data Preparation (Python)
Dilakukan oleh **Person 1 & Person 2** menggunakan Google Colab & pandas.

### ✔ Tahap Cleaning (Person 1 – Hardy Gustino)
- Menghapus duplikasi  
- Menangani nilai kosong (NaN)  
- Memperbaiki tipe data (int, float, string)  
- Normalisasi harga & diskon  
- Menjaga konsistensi kategori  

Output:  
`amazon_clean.csv`

---

## 📈 3. Exploratory Data Analysis (Python)  
Dilakukan oleh **Person 2 – Bagas Firdaus Tri Putra**

### ✔ Tahapan EDA:
- Statistik dasar (mean, median, min, max, std)
- Distribusi harga, diskon, rating
- Korelasi awal antar variabel
- Visualisasi awal dengan matplotlib & seaborn
- Interpretasi insight awal untuk dashboard Power BI

Output:  
`columns_for_dashboard.md`  
`2_eda_visualization.ipynb`

---

## 📊 4. Dashboard in Power BI  
Dibangun oleh **Ferdi Endahas**

### KPI yang ditampilkan:
- 📦 Jumlah Produk  
- ⭐ Rata-rata Rating  
- 🎯 Rata-rata Diskon (%)  
- 🔥 Total Rating Count  

### Visualisasi Utama
1. **Diskon (%) vs Rating** (scatter plot)  
2. **Kategori Paling Laku** (bar chart: sum of rating_count)  
3. **Harga vs Rating** (scatter plot)  
4. **Rata-rata Harga & Diskon per Kategori** (combo chart)  
5. **Top Products Table** (rating + rating_count)

---

## 🔍 5. Insight Utama
### 1️⃣ Diskon tinggi ≠ Rating lebih tinggi
Produk dengan diskon 20–80% tetap berada di rating 3.8–4.3.

### 2️⃣ Kategori “In-Ear”, “USBCables”, dan “Smartphones” adalah yang paling laku
Dilihat dari rating_count tertinggi.

### 3️⃣ Harga antar kategori berbeda jauh
Kategori tertentu mahal tapi diskonnya kecil.

### 4️⃣ Harga tidak berkorelasi kuat dengan rating
Produk mahal tidak menjamin rating tinggi.

### 5️⃣ Top Products
Produk terbaik umumnya:
- rating di atas 4.3  
- rating_count sangat besar → populer & konsisten

---

## 📁 6. Struktur Repository

```
📦 project-folder
│
├── data/
│   ├── amazon_raw.csv
│   ├── amazon_clean.csv
│   └── columns_for_dashboard.md
│
├── notebooks/
│   └── 2_eda_visualization.ipynb
│
├── powerbi/
│   └── Product Rating & Sales Insights.pbix
│
└── README.md
```

---

## 👥 7. Contributors & Roles

| Nama | Role | Tanggung Jawab |
|------|------|----------------|
| **Hardy Gustino** | **Data Engineer & Data Cleaning** | Menyiapkan data, cleaning, memahami struktur dataset, membuat dataset bersih. |
| **Bagas Firdaus Tri Putra** | **EDA & Visualization Specialist (Python)** | EDA, visualisasi Python, analisis statistik, pemilihan kolom dashboard. |
| **Ferdi Endahas** | **Dashboard Developer & Documenter** | Power BI dashboard, KPI design, final layout, pembuatan README & dokumentasi portfolio. |

---

## 🛠 8. Tools yang Digunakan
- Python (pandas, numpy, matplotlib, seaborn)  
- Google Colab  
- Power BI Desktop  
- GitHub  

---

## 📸 9. Preview Dashboard

Tambahkan screenshot:  
```
![Dashboard Preview](powerbi/dashboard-preview.png)
```

---

## ▶️ 10. Cara Menjalankan
1. Clone repository:
```
git clone https://github.com/username/repo-name.git
```

2. Buka Power BI Desktop  
3. Load file:
```
powerbi/Product Rating & Sales Insights.pbix
```

4. Jika ingin mengedit data:  
Gunakan file:
```
data/amazon_clean.csv
```

---
 

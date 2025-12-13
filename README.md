# Customer Segmentation for Personalized Retail Marketing  
**Penerapan Analisis RFM, K-Means Clustering, dan FP-Growth**

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk membangun **segmentasi pelanggan berbasis data** pada perusahaan retail guna mendukung strategi **personalized marketing** yang lebih efektif dan efisien.  

Dengan memanfaatkan data transaksi historis, proyek ini mengombinasikan:
- **RFM Analysis** untuk mengukur nilai pelanggan,
- **K-Means Clustering** untuk membentuk segmen pelanggan,
- **FP-Growth (Association Rule Mining)** untuk menghasilkan rekomendasi bundling dan kampanye pemasaran.

---

## 🎯 Latar Belakang
Perusahaan retail sering menghadapi kesulitan dalam:
- memahami perilaku pelanggan secara menyeluruh,
- mengidentifikasi pelanggan bernilai tinggi,
- serta mengukur efektivitas strategi pemasaran yang dijalankan.

Tanpa segmentasi yang jelas, strategi pemasaran cenderung bersifat umum, tidak tepat sasaran, dan kurang efisien dalam meningkatkan retensi pelanggan.  
Oleh karena itu, diperlukan pendekatan **data-driven customer segmentation** sebagai dasar pengambilan keputusan bisnis.

---

## 🧠 Tujuan Analisis
1. Mengidentifikasi segmentasi pelanggan berdasarkan perilaku transaksi.
2. Menentukan pelanggan bernilai tinggi, potensial, dan berisiko churn.
3. Menyusun rekomendasi strategi pemasaran yang berbeda untuk setiap segmen.
4. Mendukung personalisasi kampanye dan optimasi alokasi budget marketing.

---

## 🗂️ Dataset
- **Sumber**: Online Retail Dataset  
- **Jenis Data**: Transaksi retail historis  
- **Jumlah Data Awal**: ±541.000 baris transaksi  
- **Atribut Utama**:
  - InvoiceNo
  - InvoiceDate
  - CustomerID
  - Country
  - Quantity
  - UnitPrice
  - Description

---

## 🛠️ Tools & Library
- **Bahasa**: Python  
- **Library Utama**:
  - `pandas`, `numpy` – data processing
  - `matplotlib`, `seaborn` – visualisasi
  - `scikit-learn` – preprocessing & clustering
  - `yellowbrick` – evaluasi jumlah cluster
  - `mlxtend` – FP-Growth & association rules

---

## 🔄 Alur Kerja Analisis
1. **Data Preparation**
   - Load dataset transaksi
2. **Data Preprocessing**
   - Menghapus duplikasi
   - Menghapus transaksi cancelled
   - Menangani missing value & nilai negatif
3. **Exploratory Data Analysis (EDA)**
   - Tren pendapatan bulanan
   - Distribusi geografis
   - Produk terlaris & paling menguntungkan
   - Pola waktu transaksi
4. **RFM Modelling**
   - Recency, Frequency, Monetary
5. **Transformasi & Standardisasi**
   - Power Transformation (Yeo-Johnson)
6. **K-Means Clustering**
   - Elbow Method & Silhouette Score
7. **FP-Growth Analysis**
   - Association rule mining untuk rekomendasi produk
8. **Business Insight & Strategy**
   - Rekomendasi pemasaran per segmen

---

## 📊 Segmentasi Pelanggan (Hasil Clustering)
Jumlah cluster optimal: **4**

| Cluster | Nama Segmen | Karakteristik Utama |
|------|-----------|-------------------|
| 0 | VIP / Champions | Sangat aktif, high spender |
| 1 | Loyalist | Aktif, nilai belanja kecil |
| 3 | At Risk | Mulai jarang belanja |
| 2 | Hibernating / Lost | Lama tidak bertransaksi |

---

## 🎯 Rekomendasi Strategi Bisnis

### 🔹 Cluster 0 – VIP
- Early access produk baru
- Program loyalitas eksklusif
- Referral program
- Reward berbasis momen (ulang tahun)

### 🔹 Cluster 1 – Loyalist
- Bundling ringan berbasis FP-Growth
- Email reminder & rekomendasi best seller
- Edukasi produk untuk meningkatkan repeat purchase

### 🔹 Cluster 3 – At Risk
- Diskon khusus & bundling agresif
- Personal message (email / notifikasi)
- Win-back campaign berbasis pola pembelian

### 🔹 Cluster 2 – Hibernating
- Soft win-back campaign
- Event-based promotion (holiday, seasonal)
- Reminder produk terakhir dibeli

---

## 🚀 Rencana Pengembangan ke Depan
- Integrasi dengan **CRM & Marketing Automation**
- Prediksi **Customer Churn** & **Customer Lifetime Value (CLV)**
- Evaluasi efektivitas kampanye menggunakan **Uplift Modeling**
- Personalisasi rekomendasi berbasis real-time data

---

## 💰 Estimasi Anggaran Implementasi
| Komponen | Estimasi |
|--------|---------|
| CRM & Marketing Automation | Rp7.000.000 |
| Prediksi Churn & CLV | Rp3.000.000 |
| Evaluasi Kampanye & Uplift | Rp1.500.000 |
| **Total** | **Rp11.500.000** |

---

## 📌 Kesimpulan
Proyek ini menunjukkan bahwa **tidak semua pelanggan memiliki nilai yang sama**.  
Dengan segmentasi pelanggan berbasis RFM dan clustering, perusahaan dapat:
- meningkatkan efektivitas pemasaran,
- mengoptimalkan alokasi budget,
- serta membangun strategi retensi pelanggan yang lebih tepat sasaran.

---

## 👥 Tim Proyek
- **Project Manager**: Muhamad Salman Alfarisi  
- **Data Engineer / Scientist**: Azzam  
- **Data Analyst / Strategist**: Rindu  

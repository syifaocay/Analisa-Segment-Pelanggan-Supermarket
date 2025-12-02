# Analisa-Segment-Pelanggan-Supermarket
Tugas ini dibuat untuk menyelesaikan Tugas Capstone 2 di Purwadhika


# Analisis Perilaku Pelanggan Supermarket  
### Mencari "High-Value Customers" & Strategi Pemasaran yang Paling Menguntungkan  

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-blue?logo=pandas&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

**Dataset**: `Supermarket Customers.csv` (2.240 baris)  
**Periode data**: 2 tahun terakhir  
**Tools**: Python • Pandas • Matplotlib • Seaborn • Plotly • SciPy  

---

## Latar Belakang & Rumusan Masalah  
Di industri retail yang sangat kompetitif, tidak semua pelanggan sama nilainya. Proyek ini bertujuan menjawab 4 pertanyaan bisnis krusial:

1. **Siapa segmen pelanggan dengan total belanja terbesar?** (profil demografis)  
2. **Seberapa kuat pengaruh pendapatan (Income) terhadap total belanja?**  
3. **Kategori produk mana yang paling berkontribusi terhadap pendapatan supermarket?**  
4. **Kampanye pemasaran mana yang paling efektif mendorong pengeluaran pelanggan?**

---

## Temuan Utama (Key Insights)

| No | Insight | Nilai Bisnis |
|----|----------------------------------------------------------------|--------------------|
| 1 | **High Spender (Top 20%)** didominasi usia 40–69 tahun, lulusan Sarjana/PhD, sudah menikah, income ≥ €60.000 | Fokus targeting & akuisisi ke segmen ini |
| 2 | Korelasi Income ↔ Total Spending = **0.79 (sangat kuat)** | Income adalah prediktor terbaik perilaku belanja tinggi |
| 3 | **Wine (50,2%) + Daging Premium (27,6%)** = **77,8% total pendapatan** | Supermarket ini sebenarnya "Wine & Premium Meat Specialist" |
| 4 | **Kampanye 5** paling efektif → rata-rata belanja **€1.617** per pelanggan yang menerima | Jadikan template kampanye mendatang |

---

## Hasil Analisis Kampanye Pemasaran  
(Ranking berdasarkan rata-rata belanja pelanggan yang menerima kampanye)

| Rank | Kampanye         | Acceptance Rate | Rata-rata Belanja (yang menerima) |
|------|------------------|------------------|------------------------------------|
| 1    | **Kampanye 5**   | 7.2%            | **€1.617**                         |
| 2    | Kampanye 1       | 6.4%            | €1.484                             |
| 3    | Kampanye 2       | 1.3%            | €1.308                             |
| 4    | Kampanye 4       | 7.5%            | €1.143                             |
| 5    | Kampanye Terakhir| 14.9%           | €988                               |
| 6    | Kampanye 3       | 7.3%            | €721                               |

> **Kesimpulan**: Kampanye 5 adalah juara mutlak. Kampanye Terakhir menarik banyak respons, tapi tidak menghasilkan belanja tinggi.

---

## Rekomendasi Bisnis (Actionable)

1. **Targeting tajam** → 80–90% budget marketing untuk usia 40–69, berpendidikan tinggi, income ≥ €60k  
2. **Alokasi shelf & promosi** → 80% untuk Wine & Daging Premium  
3. **Replikasi Kampanye 5** sebagai template standar semua promosi mendatang  
4. **Evaluasi ulang Kampanye Terakhir** (terlalu generik) & tingkatkan daya tarik Kampanye 2  
5. Pertahankan kanal **toko fisik + katalog** (segmen utama masih aktif di sini)

---

## Struktur Notebook (`cekdata.ipynb`)

- Latar Belakang & Rumusan Masalah  
- Data Understanding + Data Dictionary  
- Exploratory Data Analysis (EDA)  
- Analisis Demografis High Spender  
- Hubungan Income vs Total Spending  
- Kontribusi Pendapatan per Kategori Produk  
- Analisis Efektivitas 6 Kampanye Pemasaran  
- Kesimpulan & Rekomendasi Bisnis  

---

## Cara Menjalankan Proyek Ini

```bash
# 1. Clone repository
git clone https://github.com/username/nama-repo.git
cd nama-repo

# 2. (Opsional) Buat virtual environment
python -m venv venv
source venv/bin/activate    # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install pandas numpy matplotlib seaborn plotly scipy

# 4. Jalankan notebook
jupyter notebook cekdata.ipynb

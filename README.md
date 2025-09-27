# Final Task – Big Data Analytics 

Repositori ini berisi pengerjaan **Final Task Program PBI Rakamin Academy x Kimia Farma**.  
Project ini mencakup integrasi dataset Kimia Farma ke Google BigQuery, pembuatan tabel analisa menggunakan SQL, serta visualisasi insight bisnis melalui Google Looker Studio.

---

## 📂 Struktur Repository
- `queries/` → berisi query SQL untuk pembuatan tabel analisa dan agregasi.  
- `README.md` → panduan singkat dan dokumentasi proses pengerjaan.  

---

## 🗂 Dataset
Dataset yang digunakan dalam project ini terdiri dari 4 file CSV:  
1. `kf_final_transaction.csv` → data transaksi Kimia Farma.  
2. `kf_inventory.csv` → data stok persediaan cabang.  
3. `kf_kantor_cabang.csv` → data kantor cabang (lokasi, kota, provinsi, rating).  
4. `kf_product.csv` → data produk (kategori, harga, nama produk).  

Seluruh dataset di-*import* ke **Google BigQuery** dalam 1 dataset bernama `kimia_farma`.

---

## ⚙️ Langkah Pengerjaan
1. **Import Data ke BigQuery**  
   Mengunggah keempat dataset (transaction, inventory, cabang, product) ke dalam BigQuery.  

2. **Integrasi Data (SQL Query)**  
   Membuat *tabel analisa* dengan menggabungkan 4 tabel utama menggunakan query SQL.  
   Tabel ini berisi informasi lengkap seperti:
   - transaksi (ID, tanggal, customer)  
   - cabang (ID, kota, provinsi, rating)  
   - produk (nama, kategori, harga)  
   - perhitungan tambahan (nett_sales, nett_profit, rating_transaksi).  

4. **Perhitungan Analisis**
   - *Nett Sales* = harga produk – diskon.  
   - *Nett Profit* = nett sales × persentase gross laba (berdasarkan kategori harga).  
   - *Rating Transaksi* = skor performa dari data transaksi.  

6. **Visualisasi Dashboard**  
   Menghubungkan tabel analisa di BigQuery dengan **Google Looker Studio**, lalu membuat dashboard interaktif yang menampilkan:
   - total penjualan dan profit  
   - top produk dan cabang  
   - distribusi transaksi per provinsi  
   - tren performa bisnis Kimia Farma.  

---

## 📊 Dashboard
👉 [Lihat Dashboard Google Looker Studio](https://lookerstudio.google.com/reporting/b749e4e5-f157-48e0-b29f-839d1c63a9a9/page/oQjZF/edit)

---

## 👨‍💻 Kontributor
Aya Reggyna Octavia – Peserta Program PBI Big Data Analytics Rakamin Academy x Kimia Farma

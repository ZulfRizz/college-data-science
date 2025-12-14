# Tahapan 1: Business Understanding

Fase **Business Understanding** adalah langkah paling awal dan paling krusial dalam siklus hidup proyek data science, sebagaimana didefinisikan dalam metodologi CRISP-DM. Tujuan utamanya adalah untuk memastikan bahwa proyek yang akan dikerjakan benar-benar selaras dengan kebutuhan bisnis dan dapat memberikan nilai tambah yang nyata.

Fase ini berfokus pada tiga pilar utama:
1.  **Menentukan Tujuan Bisnis**: Memahami "apa" dan "mengapa" dari masalah yang ingin diselesaikan.
2.  **Menilai Situasi dan Kondisi**: Menginventarisasi sumber daya, batasan, dan risiko.
3.  **Membuat Rencana Proyek**: Menyusun kerangka kerja dan langkah-langkah awal.

---

## 1.1 Menentukan Tujuan Bisnis (Determine Business Objectives)

Langkah ini adalah tentang menerjemahkan masalah bisnis menjadi tujuan yang jelas dan terukur. Tanpa tujuan yang jelas, tim data science akan bekerja tanpa arah.

### 1.1.1 Memahami Latar Belakang Bisnis
Sebelum mendefinisikan tujuan, penting untuk memahami konteksnya. Tim proyek perlu menggali informasi mengenai:
- **Situasi Bisnis Saat Ini**: Apa masalah yang sedang dihadapi? (Contoh: Tingkat *churn* pelanggan meningkat dalam dua kuartal terakhir).
- **Struktur Organisasi**: Departemen mana yang akan terpengaruh oleh proyek ini? Siapa saja pemangku kepentingan (stakeholders) utamanya?
- **Peluang Bisnis**: Apa peluang yang bisa didapatkan jika masalah ini teratasi? (Contoh: Menghemat biaya akuisisi pelanggan baru dengan mempertahankan pelanggan lama).

### 1.1.2 Merumuskan Tujuan Bisnis yang SMART
Tujuan yang baik haruslah **SMART**:
- **Specific (Spesifik)**: Tujuan harus jelas. *Bukan "Meningkatkan penjualan", tetapi "Meningkatkan penjualan produk kategori X pada segmen pelanggan Y."*
- **Measurable (Terukur)**: Harus ada metrik untuk mengukur keberhasilan. *Bukan "Mengurangi churn", tetapi "Menurunkan churn rate dari 5% menjadi 3%."*
- **Achievable (Dapat Dicapai)**: Tujuan harus realistis dengan sumber daya yang ada.
- **Relevant (Relevan)**: Tujuan harus mendukung strategi bisnis perusahaan yang lebih besar.
- **Time-bound (Terikat Waktu)**: Harus ada tenggat waktu yang jelas. *"Target harus tercapai dalam 6 bulan ke depan."*

### 1.1.3 Menentukan Kriteria Keberhasilan Bisnis
Ini adalah metrik akhir yang digunakan oleh pemangku kepentingan untuk menilai apakah proyek berhasil atau tidak. Kriteria ini harus dinyatakan dalam bahasa bisnis, bukan bahasa teknis.

- **Contoh Kriteria Teknis (Bukan Kriteria Bisnis)**: "Model prediksi memiliki akurasi 95%."
- **Contoh Kriteria Keberhasilan Bisnis**: "Proyek dianggap berhasil jika mampu memberikan daftar 1000 pelanggan paling berisiko *churn* setiap bulannya, dan dari daftar tersebut, tim retensi berhasil mempertahankan minimal 15% di antaranya."

---

## 1.2 Menilai Situasi dan Kondisi (Assess Situation)

Setelah tujuan ditetapkan, langkah selanjutnya adalah melakukan "uji realitas" dengan menilai semua faktor internal dan eksternal yang dapat memengaruhi proyek.

### 1.2.1 Inventarisasi Sumber Daya
- **Data**: Data apa saja yang tersedia? Di mana disimpannya (database, file, API)? Apakah ada kamus data? Siapa penanggung jawab data tersebut?
- **Personel**: Siapa saja yang memiliki keahlian yang dibutuhkan? (Ahli domain, Data Engineer, Data Analyst). Apakah keahlian mereka tersedia untuk proyek ini?
- **Infrastruktur & Alat**: Platform komputasi (Cloud/On-premise), *software*, dan *library* apa yang tersedia dan akan digunakan?

### 1.2.2 Analisis Batasan, Asumsi, dan Risiko
- **Batasan (Constraints)**: Faktor-faktor yang tidak bisa diubah dan harus diterima.
    - *Contoh*: Anggaran proyek maksimal \$50,000; Data pribadi pelanggan tidak boleh keluar dari server internal karena regulasi privasi.
- **Asumsi (Assumptions)**: Hal-hal yang kita anggap benar untuk melanjutkan proyek, namun perlu divalidasi.
    - *Contoh*: "Kami berasumsi data transaksi selama 1 tahun terakhir cukup untuk menangkap pola perilaku pelanggan."
- **Risiko (Risks)**: Potensi masalah yang bisa menghambat atau menggagalkan proyek.
    - *Contoh*: Kualitas data yang ternyata sangat buruk; Pemangku kepentingan utama pindah ke perusahaan lain di tengah proyek.

### 1.2.3 Analisis Biaya dan Manfaat (Cost-Benefit Analysis)
Lakukan analisis sederhana untuk membandingkan perkiraan biaya (waktu, tenaga, sumber daya) dengan potensi manfaat (peningkatan pendapatan, efisiensi operasional, penghematan biaya). Ini membantu memastikan bahwa proyek ini layak secara finansial.

---

## 1.3 Membuat Rencana Proyek (Produce Project Plan)

Ini adalah langkah terakhir dalam fase *Business Understanding*, di mana semua informasi yang telah dikumpulkan dirangkum menjadi sebuah rencana awal.



### 1.3.1 Rencana dan Jadwal Proyek
Buat garis besar tahapan-tahapan proyek (mengacu pada CRISP-DM) beserta estimasi waktu untuk setiap tahapannya. Rencana ini akan menjadi panduan bagi seluruh tim.
- **Fase 1: Business Understanding** (1-2 minggu)
- **Fase 2: Data Understanding** (2-3 minggu)
- **Fase 3: Data Preparation** (3-5 minggu)
- **dst.**

### 1.3.2 Definisi *Deliverables*
Tentukan apa saja hasil kerja (output) yang akan diserahkan pada setiap akhir tahapan. Contohnya, *deliverable* dari fase *Business Understanding* adalah dokumen rencana proyek ini sendiri.

### 1.3.3 Pemilihan Alat dan Teknik Awal
Berdasarkan tujuan dan sumber daya, buat daftar awal mengenai alat dan teknik yang kemungkinan akan digunakan.
- **Tujuan**: Prediksi Churn (Klasifikasi Biner)
- **Potensi Teknik**: Regresi Logistik, Random Forest, XGBoost.
- **Potensi Alat**: Python dengan library Scikit-learn, Jupyter Notebook untuk eksplorasi, SQL untuk pengambilan data.

Dengan menyelesaikan tiga pilar ini, proyek data science Anda memiliki fondasi yang kuat untuk melangkah ke fase teknis berikutnya. 🚀
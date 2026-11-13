E-Commerce Data Analysis: Product & Customer Insights (TheLook)

Tujuan Project

Proyek ini bertujuan untuk menganalisis kinerja penjualan, distribusi inventaris produk, serta status pemesanan pelanggan di TheLook E-Commerce. Hasil analisis ini dirancang untuk membantu tim Manajemen (Product, Marketing, dan CRM) dalam merancang strategi promosi produk premium, mengoptimalkan stok kategori terlaris, serta mengevaluasi tingkat keberhasilan pengiriman pesanan.
Dataset

Dataset yang digunakan adalah dataset publik e-commerce berskala besar dari Google BigQuery.

    Sumber Data: bigquery-public-data.thelook_ecommerce

    Tabel yang Digunakan:

        products (Katalog data produk)

        users (Data demografi pelanggan)

        orders (Data pesanan pelanggan)

        order_items (Detail item transaksi)

Pertanyaan Bisnis

Analisis ini difokuskan untuk menjawab lima pertanyaan strategis dari berbagai departemen:

    Analisis Produk: Bagaimana karakteristik katalog produk yang dijual? (Fokus pada 20 produk pertama).

    Identifikasi Produk Premium: Apa saja produk dengan harga retail di atas $100 yang bisa difokuskan untuk kampanye VIP Marketing?

    Evaluasi Kategori Produk: Kategori produk apa yang memiliki variasi (jumlah produk) paling banyak di dalam inventaris?

    Mengenal Pelanggan & Pesanan: Bagaimana detail informasi pelanggan berserta status pemesanan mereka?

    Analisis Penjualan per Kategori: Kategori produk mana yang memberikan kontribusi total nilai penjualan terbesar?

Keterampilan SQL yang dievaluasi: SELECT, WHERE, JOIN (INNER JOIN), Agregasi (COUNT, SUM), GROUP BY, ORDER BY, dan penggunaan Alias.

Key Insights (Temuan Bisnis)

Berdasarkan hasil ekstraksi dan pengolahan data menggunakan SQL, berikut adalah temuan utama yang didapatkan:

    Dominasi Produk Premium pada Kategori Musim Dingin: Terdapat 4.002 produk dalam kategori premium (harga > $100) dengan harga tertinggi mencapai $999. Produk premium ini didominasi oleh kategori Outerwear & Coats (751 produk) dan Jeans (739 produk).

    Kesenjangan antara Kuantitas vs Pendapatan: Meskipun kategori Intimates memiliki variasi produk terbanyak di dalam katalog (2.363 produk), kategori tersebut bukan penyumbang pendapatan terbesar.

    Penyumbang Pendapatan Utama (Top Revenue Drivers): Kategori Outerwear & Coats merupakan penyumbang omzet tertinggi perusahaan dengan total penjualan mencapai ~$1,33 Juta, disusul sangat ketat oleh kategori Jeans dengan ~$1,24 Juta, dan Sweaters dengan ~$829 Ribu.

    Evaluasi Tingkat Retur dan Pembatalan (CRM): Dari total lebih dari 125.000 pesanan, meskipun pesanan sukses (Shipped & Complete) mendominasi, terdapat tingkat Cancelled (18.879 pesanan) dan Returned (12.530 pesanan) yang cukup signifikan dan memerlukan eskalasi ke tim operasional.

Rekomendasi Bisnis

    Fokus Kampanye Marketing: Tim Marketing harus mengalokasikan budget iklan (Ads) lebih besar untuk mempromosikan kategori Outerwear & Coats dan Jeans, karena kedua kategori ini tidak hanya mendominasi segmen harga premium, tetapi juga terbukti menghasilkan Gross Merchandise Value (GMV) tertinggi.

    Optimasi Inventaris: Tim Product perlu meninjau ulang stok produk Intimates. Mengingat jumlah variasinya sangat tinggi namun bukan penyumbang omzet utama, perusahaan mungkin menanggung biaya penyimpanan (holding cost) yang kurang efisien.

    Investigasi CX & Logistik (CRM): Dengan adanya lebih dari 31.000 pesanan yang dibatalkan atau dikembalikan, Tim CRM dan Operasional perlu melakukan survei kepuasan pelanggan terkait alasan retur (apakah masalah ukuran baju, cacat produk, atau keterlambatan logistik).

Project ini dikerjakan oleh Muhammad Ihsan Aulia Rahman sebagai portofolio Data Analytics.

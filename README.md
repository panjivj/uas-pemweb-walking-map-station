### Deskripsi Aplikasi	:
Proyek aplikasi ini bertujuan untuk membuat peta isochrone yang memvisualisasikan waktu tempuh berjalan kaki ke stasiun kereta api. Isochrone adalah poligon yang menunjukkan area yang dapat dijangkau dari suatu titik (stasiun) dalam waktu tertentu

###  Manfaat dan relevansi	:
Proyek ini relevan untuk
•	Analisis aksesibilitas transportasi publik, khususnya bagi pejalan kaki
•	Perencanaan tata kota untuk mengidentifikasi area yang kurang terhubung dengan stasiun
•	Studi mitigasi bencana (misalnya: rute evakuasi gempa bumi)
•	Memberikan informasi ke pada public untuk estimasi waktu tempuh jalan kakai ke stasiun

### Teknologi dan Metodologi
•	Tools Utama:
o	QGIS: Digunakan untuk pemrosesan data geospasial dan pembuatan peta dasar.
o	QGIS2Web: Plugin untuk mengekspor peta ke format web (HTML, CSS, JS) sehingga hasilnya dapat diakses melalui browser.
•	Data yang Digunakan:
o	Data OpenStreetMap (OSM) untuk jaringan jalan dan lokasi stasiun.
o	Query Overpass API untuk mengekstrak data spesifik seperti jalan setapak, tangga, dan titik masuk stasiun 
•	Metode Analisis:
o	Network Analysis: Menghitung jarak tempuh berdasarkan jaringan jalan, bukan jarak lurus (as-the-crow-flies)
o	Alpha Shape Algorithm: Membuat poligon isochrone yang sesuai dengan jaringan jalan

### Kelebihan Proyek
•	Integrasi dengan GIS: Memanfaatkan QGIS yang populer di kalangan peneliti geospasial
•	Aplikasi Praktis: Cocok untuk studi kasus seperti analisis aksesibilitas stasiun MRT
Keterbatasan
•	Ketergantungan pada OSM: Kualitas hasil bergantung pada kelengkapan data OpenStreetMap. Jika jaringan jalan atau titik stasiun tidak akurat, peta isochrone akan bias
•	Skala Terbatas: Proyek ini fokus pada stasiun tertentu dan belum mencakup analisis multi-modal (misalnya kombinasi jalan kaki + transportasi umum)
•	Visualisasi Dasar: Hasil ekspor QGIS2Web mungkin kurang interaktif dibandingkan framework web modern seperti Leaflet atau Mapbox
Potensi Pengembangan
•	Integrasi API Real-Time: Menambahkan data real-time seperti kepadatan pejalan kaki atau kondisi lalu lintas
•	Analisis Multikriteria: Mempertimbangkan faktor tambahan seperti topografi, keamanan jalan, atau fasilitas publik
•	Aplikasi untuk Mitigasi Bencana: Mengadaptasi metodologi ini untuk merancang rute evakuasi gempa bumi, seperti yang dilakukan dalam penelitian sesar Lembang\

### Kesimpulan
Proyek Aplikasi Estimasi Waktu Tempuh Jalan Kaki Ke Stasiun merupakan solusi sederhana namun powerful untuk analisis aksesibilitas transportasi. Meski masih memiliki keterbatasan teknis, proyek ini layak dikembangkan sebagai alat pendukung keputusan dalam perencanaan kota atau mitigasi bencana

### Peta Isochrone Waktu Tempuh Berjalan Kaki ke Stasiun

- Clone / Download project ini
- Buka dengan QGIS

### QGIS2Web

- Hasil Export QGIS2Web ada di Folder docs
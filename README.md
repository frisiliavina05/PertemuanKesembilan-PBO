# Pertemuan Kesembilan-PBO
Pada pertemuan kali ini mengimplementasikan penerapan JasperReports dalam aplikasi Java Swing yang terhubung dengan database PostgreSQL. Melalui aplikasi ini, pengguna dapat menampilkan, mencetak, serta mengekspor laporan data secara langsung dari antarmuka grafis (GUI). Laporan didesain menggunakan file .jrxml sebagai template utama, lalu dikompilasi menjadi file .jasper untuk diisi dengan data dari database. Integrasi antara JasperReports dan Java Swing dilakukan dengan memanfaatkan JasperViewer, sehingga laporan dapat ditampilkan dan dicetak langsung dari aplikasi tanpa perlu proses ekspor manual terlebih dahulu.

# JasperReports
JasperReports adalah sebuah library open-source berbasis Java yang digunakan untuk membuat laporan data secara profesional dan interaktif. Library ini mampu menampilkan laporan di aplikasi Java, mencetaknya, atau mengekspornya ke berbagai format seperti PDF, Excel, HTML, dan CSV. JasperReports sangat fleksibel karena mendukung layout dinamis, grafik, subreport, serta pengelompokan data, sehingga cocok digunakan pada sistem informasi akademik, keuangan, maupun bisnis.

Pembuatan laporan dimulai dari file template (.jrxml) yang berisi struktur desain, field data, parameter, serta query SQL untuk mengambil data dari database. File ini kemudian dikompilasi menjadi file .jasper, yang siap digunakan di aplikasi Java. Selanjutnya, data diisi ke laporan menggunakan JasperFillManager, menghasilkan objek JasperPrint yang bisa ditampilkan menggunakan JasperViewer atau diekspor ke berbagai format. Melalui integrasi ini, pengguna dapat mengatur parameter laporan, menampilkan hasilnya langsung di GUI, serta mencetak laporan sesuai kebutuhan.

# Fitur Utama
- Mendukung penggunaan parameter dan query dinamis dari database.
- Dapat diintegrasikan ke aplikasi berbasis Java Swing maupun Java Web.
- Menyediakan berbagai format output: PDF, Excel, HTML, CSV, XML, dan lainnya.
- Mendukung visualisasi data melalui grafik, subreport, serta grouping data.
- Mempermudah pembuatan laporan tanpa perlu menulis layout secara manual di kode Java.

# Komponen Penting
- .jrxml → Template laporan berbasis XML yang berisi desain dan query data.
- .jasper → Hasil kompilasi dari file .jrxml yang siap digunakan di Java.
- JasperReport → Objek laporan hasil kompilasi.
- JasperPrint → Objek laporan yang sudah terisi data, siap ditampilkan atau dicetak.
- JasperViewer → Komponen untuk menampilkan laporan di dalam aplikasi Java Swing.

# Cara Instalasi
1. Buka menu Tools di NetBeans. <br>
2. Pilih Plugins → Downloaded → Add Plugins.... <br>
3. Tambahkan plugin iReport dan org.jdesktop.layout, lalu lakukan instalasi.<br>
4. Masukkan library JasperReports ke dalam project Java (contoh: jasperreports-x.x.x.jar). <br>
5. Tambahkan dependensi pendukung seperti groovy-all.jar, commons-logging.jar, commons-collections.jar, dan lainnya. <br>
6. Pastikan driver JDBC sesuai dengan database yang digunakan (misalnya postgresql-xx.jar). <br>

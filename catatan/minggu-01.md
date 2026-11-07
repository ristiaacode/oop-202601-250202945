# Catatan Minggu 1: Paradigma Pemrograman dan Setup

## Yang saya kerjakan
Minggu ini saya menyiapkan environment development dengan mengunduh dan mengonfigurasi JDK 21 serta Apache Maven. Kemudian dilanjut dengan memperbarui file `mahasiswa.properties` dengan memasukkan nama dan NIM saya. Saya menyelesaikan tugas membuat program sapaan di Java menggunakan tiga paradigma berbeda yaitu, prosedural, OOP, dan fungsional. Terakhir, saya menguji semua fungsi program dengan script yang telah disediakan.

## Keputusan desain
Supaya lolos unit test, saya menyamakan format output sapaan di ketiga paradigma menjadi, `"Halo, " + nama + "(" + nim + ") selamat datang di Aset-Pinjam!"`.

## Kendala
Terminal sempat tidak mengenali perintah `mvn` saat setup Environment Variables. Ternyata PATH saya malah mengarah ke folder shortcut (`javapath`), bukan ke folder instalasi aslinya. Masalah ini selesai setelah saya pathing ulang `JAVA_HOME` dan `MAVEN_HOME` langsung ke lokasi instalasi di `Program Files`, lalu me-restart terminal.

## Penggunaan AI
- Alat yang dipakai: Gemini
- Bagian yang dibantu AI: Setup Environment (JDK 21 & Maven) dan penjelasan dari ketiga kelas paradigma.
- Prompt utama:
1. "bagaimana cara setup maven"
2. "penjelasan mengenai ketiga kelas paradigma pemrograman dan setup"
- Yang saya ubah atau tolak dari saran AI, dan alasannya:
Untuk minggu ini, penjelasan dari AI sudah tepat. Saya hanya menyesuaikan format kalimat sapaan pada kode Java agar tetap ringkas.
- Satu hal yang saya pahami lebih baik sekarang:
Saya jadi lebih paham mengenai perbedaan mendasar dari ketiga paradigma di Java terutama bagaimana ekspresi lambda di paradigma fungsional bisa melempar fungsi sebagai nilai tanpa harus membuat kelas pembungkus secara manual seperti di OOP.
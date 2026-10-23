# Catatan Minggu 1: Paradigma Pemrograman dan Setup

## Yang saya kerjakan
Saya melakukan setup environment untuk memasang JDK 21 dan Apache Maven serta mengkonfigurasi variabel lingkungannya, kemudian saya mengisi nama dan nim pada file mahasiswa.properties. Saya melengkapi implementasi program sapaan menggunakan tiga paradigma pemrograman berbeda di Java, yaitu prosedural, Object-Oriented Programming (OOP), dan fungsional. saya juga menguji seluruh fungsi program menggunakan script pengujian yang disediakan.

## Keputusan desain
Saya memutuskan untuk membuat format kalimat sapaan yang konsisten di ketiga kelas paradigma, yaitu `"Halo, " + nama + "(" + nim + ") selamat datang di Aset-Pinjam!"` agar lulus dalam pengujian. 

## Kendala
Saat konfigurasi Environment Variables (PATH) untuk JDK 21 dan Maven, terminal sempat tidak mengenali perintah `mvn` karena variabel mengarah ke lokasi shortcut (`javapath`) dan folder yang salah. Saya mengatasinya dengan melacak direktori asli instalasi JDK dan Maven di `Program Files`, memperbarui `JAVA_HOME` dan `MAVEN_HOME`, serta membuka kembali terminal baru agar perubahan konfigurasi dimuat dengan benar.

## Penggunaan AI
- Alat yang dipakai: Gemini
- Bagian yang dibantu AI: Setup Environment (JDK 21 & Maven),penjelasan ketiga kelas paradigma
- Prompt utama:
1. "bagaimana setup maven"
2. "penjelasan ketiga kelas paradigma"
- Yang saya ubah atau tolak dari saran AI, dan alasannya:
Saya menyesuaikan format kalimat sapaan pada kode Java agar tetap ringkas.
- Satu hal yang saya pahami lebih baik sekarang:
Saya memahami perbedaan mendasar antara tiga paradigma di Java (prosedural, OOP, dan fungsional), terutama bagaimana ekspresi lambda pada gaya fungsional dapat mengembalikan fungsi sebagai nilai tanpa perlu membuat kelas pembungkus secara manual seperti pada OOP.
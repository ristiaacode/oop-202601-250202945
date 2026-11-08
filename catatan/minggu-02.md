# Catatan Minggu 02: Struktur OOP: Class, Object, Encapsulation
## Yang saya kerjakan
Mengubah beberapa kode di file `Aset.java` dengan menambahkan field private seperti `kode`, `nama`, `status`, `kondisi`. Mengimplementasikan konstruktor dengan validasi untuk memastikan `kode` dan `nama` tidak `null` atau kosong, serta memberikan nilai default `status (TERSEDIA)` dan `kondisi (BAIK)`. Membuat method getter untuk seluruh field dan setter untuk `nama`, `status`, dan `kondisi` tanpa membuat setter pada `kode` agar memenuhi aturan immutable. Juga menambahkan validasi `null` pada setter `status` dan `kondisi`, serta validasi string kosong pada setter `nama`. Serta telah lolos pengujian pada `Minggu02AsetTest.java`.

## Keputusan desain
Melakukan `.trim()` pada parameter `kode` dan `nama` saat dimasukkan melalui konstruktor atau `setNama` untuk mencegah string yang hanya berisi spasi lolos dari validasi kosong, sekaligus merapikan data. Semua atribut dibuat `private` dan akses keluar dibatasi menggunakan getter serta setter yang terkontrol. Sesuai aturan, field `kode` tidak diberikan setter agar nilainya tetap konsisten setelah objek diinisialisasi.

## Kendala
Sempat mengalami error dan tidak bisa jalan karena field private belum didefinisikan sebelumnya di dalam class `Aset.` Mengatasinya dengan mendeklarasikan field-field tersebut secara benar di awal class agar konstruktor dan method getter atau setter bisa mengaksesnya.

## Penggunaan AI
- Alat yang dipakai: Gemini
- Bagian yang dibantu AI: Penjelasan mengenai Class, Object, Encapsulation beserta fungsi setiap bagian kode.
- Prompt utama: "bantu aku untuk menjelaskan Class, Object, Encapsulation"
- Yang saya ubah atau tolak dari saran AI, dan alasannya:
Tidak ada yang ditolak untuk saat ini, saya menerima saran penjelasan dari AI dan menyesuaikannya langsung dengan struktur project praktikum saya.
- Satu hal yang saya pahami lebih baik sekarang: Cara menerapkan enkapsulasi secara tepat di Java dengan memilih atribut mana yang boleh diubah via setter contohnya `nama`, `status`, `kondisi` dan mana yang harus dibuat tetap terkunci setelah objek dibuat semacam `kode`.
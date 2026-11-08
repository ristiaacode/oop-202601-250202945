# Catatan Minggu 03: Inheritance



## Yang saya kerjakan
Pada minggu ini, saya membuat hierarki class untuk sistem peminjaman aset dengan menerapkan konsep inheritance. Saya mengimplementasikan class turunan 'Ruang', 'Laptop', dan 'AlatLab' yang mewarisi class induk 'Aset' menggunakan kata kunci extends. Selain itu, saya menambahkan konstruktor yang memanggil 'super()', menerapkan validasi atribut khusus di masing-masing subclass, dan meng-override method 'getJenis()'.

## Keputusan desain
Saya memutuskan untuk menempatkan atribut umum—seperti kode dan nama aset—di class induk 'Aset' agar tidak terjadi pengulangan kode. Sementara itu, atribut spesifik seperti 'kapasitas' untuk 'ruang', 'spesifikasi' dan 'nomorInventaris' untuk laptop, serta 'laboratorium' dan 'tingkatRisiko' untuk alat lab ditempatkan di subclass masing-masing. Saya juga menambahkan validasi pada setiap konstruktor subclass agar data yang dimasukkan sudah tervalidasi sebelum objek dibuat.

## Kendala
Kendala utama saya adalah memastikan cara memanggil konstruktor induk dengan benar menggunakan 'super(...)' sekaligus menambahkan validasi input, seperti pengecekan string kosong dan nilai kapasitas. Masalah ini teratasi setelah saya mempelajari kembali cara kerja konstruktor di subclass serta menambahkan pengecekan 'null' dan 'trim().isEmpty()' pada parameter input.

## Penggunaan AI
- Alat yang dipakai: (nama, atau "tidak memakai")
- Bagian yang dibantu AI: Penjelasan materi inheritance dan panduan pengerjaan tugas terkait.
- Prompt utama:
1. "Bantu aku untuk menjelaskan materi Inheritance, dan jelaskan tugas tersebut"
- Yang saya ubah atau tolak dari saran AI, dan alasannya:
Saya menerima penjelasan konsep dan arahan struktur kode yang diberikan AI untuk diimplementasikan sendiri ke dalam class 'Ruang', 'Laptop', dan 'AlatLab'.
- Satu hal yang saya pahami lebih baik sekarang:
Saya jadi jauh lebih paham fungsi keyword 'super' untuk meneruskan data ke class induk, serta fungsi anotasi '@Override' sebagai pengaman dari compiler untuk memastikan method turunan benar-benar menimpa method induk dengan tepat.
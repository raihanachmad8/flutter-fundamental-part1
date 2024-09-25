Nama   : Achmad Raihan Fahrezi Effendy \
NIM    : 2241720192 \
Kelas  : TI-3D

<h3 style="text-align: center; font-weight: bold;">
Widget Dasar Flutter
</h3>
Pada codelab ini, Anda akan mempelajari konsep dan praktik untuk dasar-dasar framework Flutter termasuk fitur penggunaan hot reload dan restart serta widget dasar dan temanya.

#### **Tujuan Praktikum**

Setelah menyelesaikan codelab ini Anda akan mampu untuk:

- menjelaskan bagian-bagian dari project file flutter
- menggunakan fitur hot reload dan restart
- menjelaskan perbedaan stateful dan stateless widget
- menerapkan widget-widget dasar flutter dan tema

---

### Praktikum 1

Membuat Project Flutter Baru

Selesaikan langkah-langkah praktikum berikut ini menggunakan editor Visual Studio Code (VS Code) atau Android Studio atau code editor lain kesukaan Anda.

> Perhatian: Diasumsikan Anda telah berhasil melakukan setup environment Flutter SDK, VS Code, Flutter Plugin, dan Android/iOS SDK pada [Codelabs#1](https://jti-polinema.github.io/flutter-codelab/01-pengenalan/).

#### Praktikum 1 - Langkah 1

Buka VS Code, lalu tekan tombol Ctrl + Shift + P maka akan tampil Command Palette, lalu ketik Flutter. Pilih New Application Project.

![alt text](/assets/pertemuan_5/output_1.png)

>Catatan: Anda dapat mengakses Command Palette dengan cara lain, yaitu pilih menu View > Command Palette. Tombol shortcut Ctrl + Shift + P mungkin hanya berlaku di Windows.

#### Praktikum 1 - Langkah 2

Kemudian buat folder sesuai style laporan praktikum yang Anda pilih. Disarankan pada folder dokumen atau desktop atau alamat folder lain yang tidak terlalu dalam atau panjang. Lalu pilih Select a folder to create the project in.

![alt text](/assets/pertemuan_5/output_2.png)

#### Praktikum 1 - Langkah 3

Buat nama project flutter hello_world seperti berikut, lalu tekan Enter. Tunggu hingga proses pembuatan project baru selesai.

![alt text](/assets/pertemuan_5/output_3.png)

>Perhatian: Nama project ini harus lowercase (huruf kecil semua) tanpa menggunakan spasi. Untuk memisahkan kata, bisa menggunakan underline (garis bawah). Nama project tidak dapat diawali dengan angka atau karakter khusus lain. Nama project ini bukan nama aplikasi yang akan tampil di Play Store atau App Store. Untuk nama aplikasi, nanti dapat diatur ketika melakukan deployment.

#### Praktikum 1 - Langkah 4

Jika sudah selesai proses pembuatan project baru, pastikan tampilan seperti berikut. Pesan akan tampil berupa "Your Flutter Project is ready!" artinya Anda telah berhasil membuat project Flutter baru.

![alt text](/assets/pertemuan_5/output_4.png)

---

### Praktikum 2

Membuat Repository GitHub dan Laporan Praktikum

Melanjutkan dari praktikum 1, silakan selesaikan langkah-langkah berikut ini.

> Perhatian: Diasumsikan Anda telah mempunyai akun GitHub dan Anda telah memahami konsep dasar dalam bekerja menggunakan Git pada pertemuan pertama.

Praktikum ini dapat Anda lewati langsung ke langkah 11 jika sudah paham cara membuat laporan praktikum sesuai style yang Anda pilih.

#### Praktikum 2 - Langkah 1

Login ke akun GitHub Anda, lalu buat repository baru dengan nama "flutter-fundamental-part1"
![alt text](/assets/pertemuan_5/output_5.png)

#### Praktikum 2 - Langkah 2

Lalu klik tombol "Create repository" lalu akan tampil seperti gambar berikut.\
![alt text](/assets/pertemuan_5/output_6.png)

#### Praktikum 2 - Langkah 3

KKembali ke VS code, project flutter hello_world, buka terminal pada menu Terminal > New Terminal. Lalu ketik perintah berikut untuk inisialisasi git pada project Anda.

```bash
git init
```

![alt text](/assets/pertemuan_5/output_7.png)

#### Praktikum 2 - Langkah 4

Pilih menu Source Control di bagian kiri, lalu lakukan stages (+) pada file .gitignore untuk mengunggah file pertama ke repository GitHub.

![alt text](/assets/pertemuan_5/output_8.png)

#### Praktikum 2 - Langkah 5

Beri pesan commit "tambah gitignore" lalu klik Commit (✔)
![alt text](/assets/pertemuan_5/output_9.png)

#### Praktikum 2 - Langkah 6

Lakukan push dengan klik bagian menu titik tiga > Push
![alt text](/assets/pertemuan_5/output_10.png)

#### Praktikum 2 - Langkah 7

Di pojok kanan bawah akan tampil seperti gambar berikut. Klik "Add Remote"
![alt text](/assets/pertemuan_5/output_11.png)

#### Praktikum 2 - Langkah 8

Salin tautan repository Anda dari browser ke bagian ini, lalu klik Add remote
![alt text](/assets/pertemuan_5/output_12.png)
Setelah berhasil, tulis remote name dengan "origin"
![alt text](/assets/pertemuan_5/output_13.png)

#### Praktikum 2 - Langkah 9

Lakukan hal yang sama pada file README.md mulai dari Langkah 4. Setelah berhasil melakukan push, masukkan username GitHub Anda dan password berupa token yang telah dibuat (pengganti password konvensional ketika Anda login di browser GitHub). Reload halaman repository GitHub Anda, maka akan tampil hasil push kedua file tersebut seperti gambar berikut.
![alt text](/assets/pertemuan_5/output_14.png)

> Perhatian: Personal access token GitHub dapat Anda buat melalui <https://github.com/settings/tokens/new> atau dapat membaca dokumentasi GitHub Token.

#### Praktikum 2 - Langkah 10

Lakukan push juga untuk semua file lainnya dengan pilih Stage All Changes. Beri pesan commit "project hello_world". Maka akan tampil di repository GitHub Anda seperti berikut.
![alt text](/assets/pertemuan_5/output_15.png)

#### Praktikum 2 - Langkah 11

Kembali ke VS Code, ubah platform di pojok kanan bawah ke emulator atau device atau bisa juga menggunakan browser Chrome. Lalu coba running project hello_world dengan tekan F5 atau Run > Start Debugging. Tunggu proses kompilasi hingga selesai, maka aplikasi flutter pertama Anda akan tampil seperti berikut.

![alt text](/assets/pertemuan_5/output_16.png)

>Perhatian: Proses Run atau kompilasi untuk pertama kali akan memakan waktu cukup lama (3-5 menit). Namun, proses kompilasi berikutnya menjadi lebih cepat. Berbeda ketika melakukan kompilasi ke device, hal ini akan memakan waktu lebih lama lagi.

#### Praktikum 2 - Langkah 12

Silakan screenshot seperti pada Langkah 11, namun teks yang ditampilkan dalam aplikasi berupa nama lengkap Anda. Simpan file screenshot dengan nama 01.png pada folder images (buat folder baru jika belum ada) di project hello_world Anda. Lalu ubah isi README.md seperti berikut, sehingga tampil hasil screenshot pada file README.md. Kemudian push ke repository Anda.

![alt text](/assets/pertemuan_5/output_17.png)

> Perhatian: Lakukan proses screenshot seperti pada Langkah 12 untuk setiap Laporan Praktikum yang Anda akan buat pada praktikum selanjutnya hingga pertemuan project final.

---

### Tugas Praktikum

1. Selesaikan Praktikum 1 sampai 4, lalu dokumentasikan dan push ke repository Anda berupa screenshot setiap hasil pekerjaan beserta penjelasannya di file README.md!
2. Pada praktikum 4 mulai dari Langkah 3 sampai 6, buatlah file widget tersendiri di folder basic_widgets, kemudian pada file main.dart cukup melakukan import widget sesuai masing-masing langkah tersebut!
3. Selesaikan Codelabs: Your first Flutter app, lalu buatlah laporan praktikumnya dan push ke repository GitHub Anda!
4. README.md berisi: capture hasil akhir tiap praktikum (side-by-side, bisa juga berupa file GIF agar terlihat proses perubahan ketika ada aksi dari pengguna) di browser dan perangkat fisik (device) dengan menampilkan NIM dan Nama Anda sebagai ciri pekerjaan Anda. Jika mode developer di perangkat HP Anda belum aktif, silakan cari di internet cara mengaktifkannya!
5. Kumpulkan berupa link repository/commit GitHub Anda ke tautan spreadsheet yang telah disepakati oleh dosen!

#### Jawaban

1. [Klik untuk menuju Praktikum 1 - 4](#praktikum-1)
2. Fungsi dalam Dart adalah sekumpulan instruksi yang melakukan tugas tertentu. Fungsi dapat menerima input (parameter) dan mengembalikan output

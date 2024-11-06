# JOBSHEET 9 Praktikum 1

Nama: Wulan Maulidya P. F

Kelas: TI-3H

No. Absen: 27

NIM: 2241720174

---

## Langkah 1: Buat Project Baru
Buatlah sebuah project flutter baru dengan nama kamera_flutter, lalu sesuaikan style laporan praktikum yang Anda buat.

## Langkah 2: Tambah dependensi yang diperlukan
Untuk menambahkan dependensi plugin, jalankan perintah flutter pub add seperti berikut di terminal:

![Praktikum](/images/p1_langkah2a.png)

Setelah dijalankan maka akan ada update pada file pubscpec.yaml

![Praktikum](/images/p1_langkah2b.png)

## Langkah 3: Ambil Sensor Kamera dari device
Selanjutnya, kita perlu mengecek jumlah kamera yang tersedia pada perangkat menggunakan plugin camera seperti pada kode berikut ini. Kode ini letakkan dalam void main().

![Praktikum](/images/p1_langkah3a.png)

Ubah void main() menjadi async function seperti berikut ini.

![Praktikum](/images/p1_langkah3b.png)

## Langkah 4: Buat dan inisialisasi CameraController
Setelah Anda dapat mengakses kamera, gunakan langkah-langkah berikut untuk membuat dan menginisialisasi CameraController. Pada langkah berikut ini, Anda akan membuat koneksi ke kamera perangkat yang memungkinkan Anda untuk mengontrol kamera dan menampilkan pratinjau umpan kamera.

1. Buat StatefulWidget dengan kelas State pendamping.
2. Tambahkan variabel ke kelas State untuk menyimpan CameraController.
3. Tambahkan variabel ke kelas State untuk menyimpan Future yang dikembalikan dari CameraController.initialize().
4. Buat dan inisialisasi controller dalam metode initState().
5. Hapus controller dalam metode dispose().

![Praktikum](/images/p1_langkah4.png)

## Langkah 5: Gunakan CameraPreview untuk menampilkan preview foto
Gunakan widget CameraPreview dari package camera untuk menampilkan preview foto. Anda perlu tipe objek void berupa FutureBuilder untuk menangani proses async.

![Praktikum](/images/p1_langkah5.png)

## Langkah 6: Ambil foto dengan CameraController
Kode berikut letakkan dalam Widget build setelah field body.

![Praktikum](/images/p1_langkah6.png)

## Langkah 7: Buat widget baru DisplayPictureScreen
Buatlah file baru pada folder widget yang berisi kode berikut.

![Praktikum](/images/p1_langkah7.png)

## Langkah 8: Edit main.dart
Edit pada file ini bagian runApp seperti kode berikut.

![Praktikum](/images/p1_langkah8.png)

## Langkah 9: Menampilkan hasil foto
Tambahkan kode seperti berikut pada bagian try / catch agar dapat menampilkan hasil foto pada DisplayPictureScreen.

![Praktikum](/images/p1_langkah9.png)

## Deploy pada device

**Ask permission to access camera**

![Praktikum](/images/p1_langkah10a.jpg)

**Ask permission to access microphone**

![Praktikum](/images/p1_langkah10b.jpg)

**Take Picture Screen**

![Praktikum](/images/p1_langkah10c.jpg)

**Display Picture Screen**

![Praktikum](/images/p1_langkah10d.jpg)
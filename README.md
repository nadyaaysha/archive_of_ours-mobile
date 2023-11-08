# Archive Of Ours

# Apa perbedaan utama antara stateless dan stateful widget dalam konteks pengembangan aplikasi Flutter?

Stateless widget adalah widget statis yang tidak dapat berubah, sedangkan stateful widget adalah widget yang dinamis dan dapat berubah. Stateless widget biasanya digunakan untuk membuat widget atau komponen yang sederhana dan bersifat statis, sedangkan stateful widget biasanya digunakan untuk membuat widget yang memiliki data atau komponen yang akan berubah seiring waktu.

# Sebutkan seluruh widget yang kamu gunakan untuk menyelesaikan tugas ini dan jelaskan fungsinya masing-masing.

- `Scaffold`: Widget ini digunakan untuk membuat struktur dasar aplikasi Flutter. Widget ini biasanya digunakan sebagai induk dari widget lainnya.
- `AppBar`: Widget ini digunakan untuk membuat AppBar pada aplikasi Flutter. Widget ini biasanya digunakan sebagai anak dari widget `Scaffold`.
- `SingleChildScrollView`: Widget ini digunakan untuk membuat widget yang dapat discroll. Widget ini biasanya digunakan sebagai anak dari widget Scaffold.
- `Padding`: Widget ini digunakan untuk menambahkan padding pada widget lainnya.
- `Column`: Widget ini digunakan untuk membuat layout vertikal pada aplikasi Flutter. Widget ini biasanya digunakan sebagai anak dari widget `Scaffold`.
- `Row`: Widget ini digunakan untuk membuat layout horizontal pada aplikasi Flutter. Widget ini biasanya digunakan sebagai anak dari widget `Scaffold`.
- `Text`: Widget ini digunakan untuk menampilkan teks pada aplikasi Flutter.
- `Center`: Widget ini digunakan untuk membuat widget lainnya berada di tengah layar.
- `GridView.Count`: Widget ini digunakan untuk membuat layout grid pada aplikasi Flutter.
- `Material`: Widget ini digunakan untuk membuat material design pada aplikasi Flutter.
- `InkWell`: Widget ini digunakan untuk membuat area yang responsif terhadap sentuhan pada aplikasi Flutter.
- `ScaffoldMessenger`: Widget ini digunakan untuk menampilkan pesan pada aplikasi Flutter.
- `SnackBar`: Widget ini digunakan untuk menampilkan pesan singkat pada aplikasi Flutter.
- `Container`: Widget ini digunakan untuk membuat kotak pada aplikasi Flutter.
- `Icon`: Widget ini digunakan untuk menampilkan ikon pada aplikasi Flutter.

#  Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial)
 ## Membuat sebuah program Flutter baru dengan tema inventory seperti tugas-tugas sebelumnya.
 
Pertama, saya meng-generate proyek Flutter baru dengan nama archive_of_ours, kemudian saya masuk ke dalam direktori proyek tersebut. Saya membuat aplikasi saya dengan command flutter create archive_of_ours, kemudian saya masuk ke direktori aplikasi saya. Untuk menjalankan aplikasi, saya menggunakan command flutter run.

 ## Membuat tiga tombol sederhana dengan ikon dan teks dan Memunculkan Snackbar
 ### Membuat tiga tombol sederhana dengan ikon dan teks untuk:
- Melihat daftar item (Lihat Item)
- Menambah item (Tambah Item)
- Logout (Logout)
 ### Memunculkan Snackbar dengan tulisan:
- "Kamu telah menekan tombol Lihat Item ketika tombol Lihat Item ditekan.
- "Kamu telah menekan tombol Tambah Item ketika tombol Tambah Item ditekan.
- "Kamu telah menekan tombol Logout ketika tombol Logout ditekan.

- Pertama, saya akan mengubah sifat widget halaman menu menjadi stateless. Pada file main.dart, saya mengubah MyHomePage(title: 'Flutter Demo Home Page') menjadi
MyHomePage() saja dan juga menghapus const. Lal, pada file menu.dart, saya akan mengubah sifat widget halaman menjadi stateless. Saya merubah ({super.key, required this.title}) menjadi ({Key? key}) : super(key: key);. Saya juga hapus final String title dan fungsi State.

- Untuk membuat tombol dan menampilkannya, saya perlu menambahkan item-item yang dijual. Saya lakukan dengan mendefinisikan tipe pada list saya. Saya membuat class Commission yang berisi atribut name, icon, dan color. Lalu dibawah kode MyHomePage({Key? key}) : super(key: key);, saya menambahkan item-item komisi yang dijual (nama, icon, dan color item tersebut).

- Selanjutnya saya menambahkan serangkaian kode didalam Widget build yang akan menampilkan tombol (Melihat Commission, Menambah Commission, dan Logout) dari class item Commission. Disini widget wrapper saya bentuk menjadi scrollable, set padding, dan menampilkan children secara vertikal. Saya juga menampilkan text 'Archive Of Ours' dan di-set menjadi di center aplikasi. Dalam grid layout, disinilah item akan ditampilkan dari list yang berisi item-item yang telah saya buat.

- Saya membuat widget stateless baru yang akan menampilkan card agar tombol item dapat tervisualisasi. Atribut class CommissionCard ini adalah Commission. Widget build didalam class ini akan mengembalikan pop-up text (Kamu telah menekan tombol <Tombol>) yang menandakan salah satu tombol telah di-klik kapanpun user berinteraksi dengan tombolnya. Saya juga set alignment pop-up text dan paddingnya disini.

# Bonus
  ## Kamu akan mendapatkan nilai bonus pada penilaian tugas ini apabila kamu mengimplementasikan warna-warna yang berbeda untuk setiap tombol (Lihat Item, Tambah Item, dan Logout).

  Saya mengubah warna tombol dengan menambahkan atribut color di class Commission, dan saya merubah color: pada widget build class card dengan color per item-nya. Lalu pada list item saya tentukan secara manual masing-masing warna tombol.

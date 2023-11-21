# Archive Of Ours

# Tugas 9

## Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?

Bisa dlakukan pengambilan data JSON tanpa membuat model terlebih dahulu. Namun, dengan membuat model akan lebih memudahkan untuk dibaca dan mngidentifikasi bug.

## Jelaskan fungsi dari CookieRequest dan jelaskan mengapa instance CookieRequest perlu untuk dibagikan ke semua komponen di aplikasi Flutter.

CookieRequest adalah sebuah fungsi yang digunakan untuk melakukan permintaan HTTP dengan mengirimkan cookie. Instance CookieRequest perlu dibagikan ke semua komponen di aplikasi Flutter karena instance tersebut menyimpan informasi cookie yang diperlukan untuk melakukan permintaan HTTP selanjutnya.

## Jelaskan mekanisme pengambilan data dari JSON hingga dapat ditampilkan pada Flutter.

Mekanisme pengambilan data dari JSON hingga dapat ditampilkan pada Flutter, 
A.] Membuat function HTTP request dengan melakukan Uri.parse terhadap link yang mengandung JSON, 

B.] Lalu mengambilnya menggunakan get dengan tipe application/json 6789. 

C.] Setelah itu, data JSON tersebut dapat diolah dan ditampilkan pada Flutter.

## Jelaskan mekanisme autentikasi dari input data akun pada Flutter ke Django hingga selesainya proses autentikasi oleh Django dan tampilnya menu pada Flutter.

1.] User memasukkan data akunnya pada aplikasi Flutter.

2.] Aplikasi Flutter mengirimkan data akun ke server Django.

3.] Server Django memeriksa data akun yang diterima dari aplikasi Flutter.

4.] Jika data akun valid, server Django mengembalikan token ke aplikasi Flutter.

5.] Aplikasi Flutter menyimpan token yang diterima dari server Django.

6.] Aplikasi Flutter mengirimkan token ke server Django setiap kali melakukan permintaan HTTP.

7.] Server Django memeriksa token yang diterima dari aplikasi Flutter.

8.] Jika token valid, server Django mengembalikan data yang diminta oleh aplikasi Flutter.

9.] Aplikasi Flutter menampilkan menu yang diminta oleh user

## Sebutkan seluruh widget yang kamu pakai pada tugas ini dan jelaskan fungsinya masing-masing.

`MaterialApp`: Widget yang menyediakan konfigurasi tema, navigasi, dan lainnya untuk aplikasi Flutter yang menggunakan Material Design.

`Scaffold`: Widget yang menyediakan struktur layout dasar untuk aplikasi Material Design, seperti app bar, drawer, body, dan floating action button.

`AppBar`: Widget yang menampilkan app bar, yaitu sebuah panel horizontal yang biasanya berisi judul aplikasi, menu, dan aksi.

`Text`: Widget yang menampilkan teks dengan gaya tertentu.

`LeftDrawer`: Widget kustom yang dibuat untuk menampilkan drawer, yaitu sebuah panel vertikal yang dapat ditarik dari sisi kiri layar dan berisi menu navigasi.

`FutureBuilder`: Widget yang membangun dirinya sendiri berdasarkan hasil terbaru dari interaksi dengan objek Future, seperti pemanggilan web service.

`ListView`: Widget yang menampilkan daftar scrollable dari widget anak.

`Container`: Widget yang menggabungkan beberapa widget lainnya, seperti padding, margin, decoration, transform, dan lainnya.

`Column`: Widget yang menampilkan widget anak dalam arah vertikal.

`SizedBox`: Widget yang memiliki ukuran tetap dan dapat digunakan untuk memberi jarak antara widget lainnya.

`ElevatedButton`: Widget yang menampilkan tombol dengan efek elevasi dan warna latar.

`TextField`: Widget yang menampilkan bidang input teks yang dapat diedit oleh pengguna.

`Provider`: Widget yang menyediakan objek CookieRequest ke semua widget anak, sehingga memudahkan pengelolaan state dan komunikasi dengan web service.

`AlertDialog`: Widget yang menampilkan dialog yang dapat memberi informasi atau meminta konfirmasi dari pengguna.

`TextButton`: Widget yang menampilkan tombol dengan teks dan tanpa latar.

# Tugas 8

## Jelaskan perbedaan antara Navigator.push() dan Navigator.pushReplacement(), disertai dengan contoh mengenai penggunaan kedua metode tersebut yang tepat!

 `Navigator.push()` dan `Navigator.pushReplacement()` adalah dua metode navigasi yang berbeda pada Flutter. `Navigator.push()` digunakan untuk menambahkan halaman baru ke dalam tumpukan navigasi, sedangkan `Navigator.pushReplacement()` mengganti halaman teratas dalam tumpukan navigasi dengan halaman baru. Contoh penggunaan `Navigator.push()` adalah ketika pengguna ingin menavigasi ke halaman baru, seperti ketika pengguna menekan tombol "Tambahkan" pada halaman daftar item untuk menambahkan item baru. Contoh penggunaan `Navigator.pushReplacement()` adalah ketika pengguna ingin mengganti halaman saat ini dengan halaman baru, seperti ketika pengguna menekan tombol "Kembali" pada halaman detail item untuk kembali ke halaman daftar item. 

## Jelaskan masing-masing layout widget pada Flutter dan konteks penggunaannya masing-masing!
.
    * `Container`: Widget ini digunakan untuk menggabungkan beberapa widget lainnya menjadi satu widget yang dapat diatur ukurannya, posisinya, dan dekorasinya.
    * `Row`: Widget ini digunakan untuk menampilkan widget lain secara horizontal.
    * `Column`: Widget ini digunakan untuk menampilkan widget lain secara vertikal.
    * `Stack`: Widget ini digunakan untuk menampilkan widget lain secara bertumpuk.
    * `Expanded`: Widget ini digunakan untuk memperluas widget ke seluruh ruang yang tersedia.

## Sebutkan apa saja elemen input pada form yang kamu pakai pada tugas kali ini dan jelaskan mengapa kamu menggunakan elemen input tersebut!

 Elemen input pada form yang saya gunakan pada tugas kali ini adalah `TextFormField`. Saya menggunakan `TextFormField` untuk memungkinkan pengguna memasukkan teks ke dalam form. Saya memilih elemen input ini karena mereka mudah digunakan dan dapat disesuaikan dengan baik dengan kebutuhan tugas.

## Bagaimana penerapan clean architecture pada aplikasi Flutter?
 
 Penerapan clean architecture pada aplikasi Flutter melibatkan pembagian kode menjadi beberapa lapisan yang terpisah, yaitu lapisan presentasi, lapisan domain, dan lapisan data. Lapisan presentasi berisi kode yang berkaitan dengan tampilan aplikasi, seperti widget dan logika tampilan. Lapisan domain berisi kode yang berkaitan dengan logika bisnis aplikasi, seperti model dan pengontrol. Lapisan data berisi kode yang berkaitan dengan akses ke sumber daya eksternal, seperti database dan API. Dengan membagi kode menjadi lapisan yang terpisah, aplikasi menjadi lebih mudah dipelihara dan ditingkatkan, serta lebih mudah untuk diuji dan dikembangkan.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial)

![1700022419548](https://github.com/nadyaaysha/archive_of_ours-mobile/assets/124881541/15a28062-4037-4d1d-b586-4904ffcb914b)

- Saya membuat berkas baru di dalam direktori lib dengan nama commission_form.dart
- Pada berkas, saya membuat class StatefulWidget dengan nama CommissionFormPage yang mengembalikan sebuah widget Scaffold.
- Di dalam widget Scaffold terdapat appBar dengan title "Form Tambah Commission" dan body berupa widget Form.
- Di dalam widget Form, saya membuat sebuah variabel GlobalKey<FormState> untuk menyimpan state dari form. Variabel ini adalah nilai parameter key dari widget Form.
- Sesuai proyek Django sebelumnya, saya membuat lima variabel bertipe String dan int untuk menyimpan nilai input dari title, wordCount, description, genre, dan characterSource. Inisialisasi variabel-variabel ini dengan nilai "" dan 0.
- Lalu, saya membuat sebuah widget Column yang berisi tiga widget TextFormField dan satu widget ElevatedButton. Widget TextFormField untuk menerima input dari pengguna dan widget ElevatedButton untuk menangani aksi simpan data.
- Untuk setiap widget TextFormField, saya memberikan nilai parameter validator yang berupa sebuah fungsi anonim yang menerima input dari pengguna dan mengembalikan pesan error jika input tidak valid. Contoh validasi yang dapat dilakukan adalah memeriksa apakah input kosong atau tidak, dan apakah input sesuai dengan tipe data yang diharapkan.
- Untuk setiap widget TextFormField, saya memberikan nilai parameter onSaved yang berupa sebuah fungsi anonim yang menerima input dari pengguna dan menyimpannya ke variabel yang sesuai. Contoh: onSaved: (value) => name = value.
- Untuk widget ElevatedButton, saya memberikan nilai parameter onPressed yang berupa sebuah fungsi anonim yang mengecek apakah form valid atau tidak dengan menggunakan method validate() dari variabel GlobalKey<FormState>. Jika form valid, panggil method save() dari variabel tersebut untuk menyimpan data ke variabel-variabel yang sudah dibuat. Kemudian, dilakukan aksi yang diinginkan, seperti menambahkan data ke database atau kembali ke halaman sebelumnya.
- Untuk menampilkan halaman formulir tambah commission baru, saya menambahkan routing ke halaman tersebut di dalam drawer menu.

![1700022494738](https://github.com/nadyaaysha/archive_of_ours-mobile/assets/124881541/1e17e5b2-6bdd-43f0-8d56-72db4d90713a)

Ketika tombol "Tambah Commission" ditekan, aplikasi akan mengarahkan pengguna ke halaman form tambah commission baru.
- Saya menggunakan fungsi `Navigator.push` untuk melakukan navigasi ke halaman baru. Fungsi tersebut menerima dua parameter, yaitu `context` dan `MaterialPageRoute`. Parameter `context` digunakan untuk memberikan konteks pada fungsi `Navigator.push`, sedangkan parameter `MaterialPageRoute` digunakan untuk menentukan halaman yang akan ditampilkan.
- Pada parameter `MaterialPageRoute`, terdapat sebuah objek `builder` yang berisi sebuah fungsi anonim. Fungsi tersebut akan mengembalikan sebuah widget `CommissionFormPage`. Widget tersebut akan menampilkan halaman form tambah commission baru.

![1700022547236](https://github.com/nadyaaysha/archive_of_ours-mobile/assets/124881541/c20a5344-ff4f-4d0d-aeea-1695b95f9de0)

- Saya membuat fungsi showDialog() pada bagian onPressed() dari widget ElevatedButton yang berada di dalam widget Form. Fungsi ini akan menampilkan sebuah dialog atau pop-up ketika tombol ditekan.
- Selanjutnya, saya membuat  widget AlertDialog sebagai parameter builder dari fungsi showDialog(). Widget ini akan menentukan tampilan dan isi dari dialog atau pop-up yang akan muncul.
- Saya juga membuat  widget SingleChildScrollView sebagai parameter content dari widget AlertDialog. Widget ini akan membuat isi dialog atau pop-up menjadi scrollable jika terlalu panjang.
- Kemudian, saya membuat widget Column sebagai child dari widget SingleChildScrollView1. Widget ini akan menampung beberapa widget Text yang akan menampilkan data dari formulir yang diisi.
- Tidak lupa saya membuat beberapa widget Text sebagai children dari widget Column. Widget ini akan menampilkan data dari formulir yang diisi dengan menggunakan variabel-variabel yang sudah dibuat sebelumnya, seperti _title, _wordCount, _description, _genre, dan _characterSource.
- Terakhir, saya membuat sebuah widget TextButton sebagai parameter actions dari widget AlertDialog. Widget ini akan menampilkan sebuah tombol yang dapat menutup dialog atau pop-up ketika ditekan. Saya menggunakan fungsi Navigator.pop() pada bagian onPressed() dari widget TextButton untuk menutup dialog atau pop-up.

![1700022577725](https://github.com/nadyaaysha/archive_of_ours-mobile/assets/124881541/4a4a7c62-376b-4cda-a6cc-06d96af66c7e)

- Saya membuat widget LeftDrawer d dalam berkas left_drawer.dart yang mengembalikan widget Drawer sebagai hasilnya. Widget Drawer berisi widget ListView yang berisi beberapa widget ListTile sebagai opsi menu.
- Di dalamnya, saya membuat  widget DrawerHeader sebagai child pertama dari widget ListView. Widget DrawerHeader menampilkan judul dan deskripsi aplikasi.
- Saya juga membuat dua widget ListTile sebagai child selanjutnya dari widget ListView. Widget ListTile pertama akan menampilkan ikon rumah dan teks “Halaman Utama”. Widget ListTile kedua akan menampilkan ikon keranjang belanja dan teks “Tambah Commission”.
- Saya menambahkan atribut onTap pada masing-masing widget ListTile. Atribut onTap akan menentukan aksi yang dilakukan saat pengguna mengetuk opsi menu.
- Selanjutnya saya membentuk widget ListTile pertama yang akan melakukan navigasi ke halaman utama yang telah dibuat dengan widget MyHomePage.
- Untuk widget ListTile kedua, saya juga akan melakukan navigasi ke halaman form tambah commission yang dibuat dengan widget CommissionFormPage.
- Setelah membuat widget LeftDrawer, saya tambahkan widget tersebut sebagai nilai dari atribut drawer pada widget Scaffold yang digunakan untuk membuat halaman utama dan halaman form tambah commission.

# Tugas 7

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

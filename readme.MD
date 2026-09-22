Saya membuat program data product 

## Tujuan

 adalah program yang saya pelajari di pertemuan pertama/1 dan yg saya tangkap di pertemuan ini adalah untuk memahami penggunaan:

  `String`
  `int`
  `double`
  `bool`
  `DateTime`
  `List<String>`
  Perubahan nilai pada variabel
  Menampilkan data menggunakan `print()`

## Penjelasan Kode

### 1. String

```dart
String productName = 'Kopi Susu';
```

Variabel `productName` menggunakan tipe data `String` karena digunakan untuk menyimpan teks berupa nama produk.
Nilainya bisa diubah ketika dibutuhkan. Pada program ini, nama produk awalnya adalah   Kopi Susu  , kemudian diubah menjadi   Kopi Gula Aren  .

```dart
productName = 'Kopi Gula Aren';
```

Dengan menggunakan variabel, nama produk tidak perlu ditulis berulang kali pada setiap bagian program.

### 2. Integer (`int`)

```dart
int stock = 15;
```

Tipe data `int` digunakan untuk menyimpan bilangan bulat. Pada program ini, `stock` digunakan untuk menyimpan jumlah stok produk.
Nilai awal stok adalah `15`, kemudian diubah menjadi:

```dart
stock = 20;
```

### 3. Double (`double`)

```dart
double price = 18000.0;
```

`double` digunakan untuk menyimpan angka yang dapat memiliki nilai desimal. Variabel `price` digunakan untuk menyimpan harga produk ( alasan menggunakan double dikarenakan ada simbol titik atau koma untuk menandakan harga).
Harga awal produk adalah `18000.0`, kemudian diperbarui menjadi:

```dart
price = 20000.0;
```

### 4. Boolean (`bool`)

```dart
bool isAvailable = true;
```

Tipe data `bool` hanya mempunyai dua nilai, yaitu `true` dan `false`.
Pada program ini, `isAvailable` digunakan untuk menunjukkan apakah produk masih tersedia atau tidak.

Nilai awalnya:

```dart
isAvailable = true;
```

Kemudian setelah data diubah:

```dart
isAvailable = false;
```

Artinya, pada data kedua produk dianggap sudah tidak tersedia.

### 5. DateTime

```dart
DateTime updatedAt = DateTime.now();
```

`DateTime` digunakan untuk menyimpan informasi tanggal dan waktu.

Pada data awal, `DateTime.now()` digunakan untuk mengambil waktu saat program dijalankan.
Kemudian nilainya diganti dengan tanggal tertentu:

```dart
updatedAt = DateTime(2023, 10, 27);
```

Kode tersebut menghasilkan tanggal   27 Oktober 2023  .

### 6. Menampilkan Data

Data produk ditampilkan menggunakan fungsi `print()`.

Contohnya:

```dart
print('Produk: $productName');
print('Stok: $stock');
print('Harga: Rp$price');
```

Tanda `$` digunakan untuk memasukkan nilai dari sebuah variabel ke dalam teks.

Contohnya:

```dart
print('Produk: $productName');
```

Jika nilai `productName` adalah `Kopi Susu`, maka hasilnya:

```text
Produk: Kopi Susu
```

## Perubahan Data Produk

Setelah data awal ditampilkan, beberapa nilai variabel diubah:

```dart
productName = 'Kopi Gula Aren';
stock = 20;
price = 20000.0;
isAvailable = false;
updatedAt = DateTime(2023, 10, 27);
```

Bagian ini menunjukkan bahwa variabel yang sudah dibuat masih dapat diberikan nilai baru selama tipe datanya tetap sesuai.
Contohnya, `productName` yang menggunakan `String` dapat diganti dengan teks lain, sedangkan `stock` tetap harus menggunakan nilai bertipe angka bulat.

## List Bahan Produk

Program juga menggunakan `List<String>` untuk menyimpan beberapa bahan produk.

```dart
List<String> ingredients = ['Kopi', 'Susu'];
```

Pada awalnya terdapat dua bahan:

  Kopi
  Susu

Kemudian ditambahkan bahan baru menggunakan:

```dart
ingredients.add('Gula Aren');
```

Sehingga isi `ingredients` menjadi:

```text
[Kopi, Susu, Gula Aren]
```

`List` cocok digunakan ketika kita perlu menyimpan beberapa data yang memiliki tipe yang sama dalam satu variabel.

## Contoh Output

Ketika program dijalankan, hasilnya kurang lebih seperti berikut:

```text
- Data Produk Awal
Produk: Kopi Susu
Stok: 15
Harga: Rp18000.0
Tersedia: true
Update Terakhir: 2026-09-22 ...

- Data Produk Setelah Perubahan
Produk: Kopi Gula Aren
Stok: 20
Harga: Rp20000.0
Tersedia: false
Update Terakhir: 2023-10-27 00:00:00.000

Bahan-bahan: [Kopi, Susu, Gula Aren]
```

Bagian waktu pada data awal akan berbeda karena menggunakan `DateTime.now()`, sehingga mengikuti waktu ketika program dijalankan.

## Kesimpulan

Dari program yang saya buat ini dapat dilihat bahwa Dart menyediakan beberapa tipe data dasar yang dapat digunakan sesuai kebutuhan. `String` digunakan untuk teks, `int` untuk bilangan bulat, `double` untuk angka desimal, `bool` untuk kondisi benar atau salah, dan `DateTime` untuk menyimpan tanggal serta waktu.
Program ini juga memperlihatkan bahwa nilai sebuah variabel dapat diperbarui selama tipe datanya sesuai. Selain itu, `List` dapat digunakan untuk mengelompokkan beberapa data dalam satu variabel, seperti daftar bahan pada produk.


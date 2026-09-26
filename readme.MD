NAMA : FIKRI BINTANG PURNOMO
NIM : 1122140142

Pertemuan 1

void main() {
  String productName = 'Kopi Susu';
  int stock = 15;
  double price = 18000.0;
  bool isAvailable = true;
  DateTime updatedAt = DateTime.now();

  print('--- Data Produk Awal ---');
  print('Produk: $productName');
  print('Stok: $stock');
  print('Harga: Rp$price');
  print('Tersedia: $isAvailable');
  print('Update Terakhir: $updatedAt');

  // Perubahan data produk
  productName = 'Kopi Gula Aren';
  stock = 20;
  price = 20000.0;
  isAvailable = false;
  updatedAt = DateTime(2023, 10, 27);

  print('\n--- Data Produk Setelah Perubahan ---');
  print('Produk: $productName');
  print('Stok: $stock');
  print('Harga: Rp$price');
  print('Tersedia: $isAvailable');
  print('Update Terakhir: $updatedAt');

  // Menambahkan bahan-bahan
  List<String> ingredients = ['Kopi', 'Susu'];
  ingredients.add('Gula Aren');

  print('\n--- Bahan-bahan ---');
  print(ingredients);
}
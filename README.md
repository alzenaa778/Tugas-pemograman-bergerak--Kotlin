# Katalog Buku - Kotlin Essentials

## Tujuan program
Latihan membuat model data, mengolah koleksi (filter, sort, map), dan memakai null safety di Kotlin.

## Model data
data class Book dengan properti: id, title, author, price, year, category, dan discount (nullable, karena tidak semua buku diskon).

## Logika utama
1. Validasi: judul tidak boleh kosong, harga harus lebih dari 0, diskon 1-90%.
2. Filter: menampilkan buku kategori Pemrograman.
3. Sort: mengurutkan buku dari harga akhir termurah.
4. Map: mengubah data buku menjadi teks ringkasan.

## Catatan
Bagian tersulit adalah menangani properti nullable (discount) agar program tidak error. Saya menyelesaikannya dengan elvis operator (?:) untuk nilai default dan ?.let untuk tampilan teks. Saya juga memakai partition supaya data valid dan tidak valid terpisah dalam satu langkah.

## Screenshot output
![output](output.png)
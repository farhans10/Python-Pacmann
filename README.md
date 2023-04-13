# Python Project Pacmann-Super Cashier
Farhan Satria | Analytics & Data Science | Batch 13

## Background
Andi adalah seorang pemilik supermarket besar di salah satu kota di Indonesia. Andi memiliki rencana untuk melakukan perbaikan proses bisnis, yaitu Andi akan membuat sistem kasir yang self-service di supermarket miliknya. Sehingga customer bisa langsung memasukkan item yang dibeli, dan harga item yang dibeli dan fitur yang lain.

## Feature Requirement
1. Customer membuat ID transaksi customer berikut: trnsct_123 = Transaction()
2. Kemudian, Customer memasukkan nama item, jumlah item, dan harga barang = add_item([<nama item>,<jumlah item>,<harga barang>])
3. Apabila terdapat kesalahan maka bisa update dengan metode:
      - update nama = update_item_name(<nama item>, <update nama item>)
      - update jumlah = update_item_qty(<nama item>, <update jumlah item>)
      - update harga = update_item_price(<nama item>, <update harga item>)
4. Apabila ingin batal membeli maka bisa menggunakan metode:
      - menghapus item = delete_item(<nama item>)
      - menghapus seluruh transaksi = reset_transaction()
5. Apabila sudah selesai tetapi ragu apakah ada kesalahan pada input, maka customer bisa menggunakan metode check_order():
      - apabila tidak ada kesalahan maka akan mengeluarkan **"Pesanan sudah benar"**
      - apabila ada kesalahan maka akan mengeluarkan **"Terdapat kesalahan pada input"**
      - keluarkan output transaksi dari apa saja yang sudah dibeli
6. Setelah melakukan pengecekan, customer bisa mengetahui berapa total harga barang yang sudah dibeli. Metode yang digunakan adalah total_price(), terdapat ketentuan:
      - Jika total belanja > Rp.200.000 maka dapat diskon 5%
      - Jika total belanja > Rp.300.000 maka dapat diskon 8%
      - Jika total belanja > Rp.500.000 maka dapat diskon 10%
      
## Flowchart
Flowchart dari program Super Cashier adalah sebagai berikut :
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/Flow%20Chart%20Cashier%20Project.jpg?raw=true)

## Penjelasan File dan Attribute
Program ini hanya menggunakan 1 file, dimana terdapat class Transaction yang berisi fungsi-fungsi dengan penjelasan sebagai berikut:
1. def __init__(self): berfungsi untuk inisialisasi atribut keranjang yang berfungsi sebagai list kosong untuk menampung item yang akan dibeli
2. def add_item(self): berfungsi untuk menambahkan barang yang kemudian akan ditampung di keranjang
3. def update_nama_item(self): berfungsi untuk mengubah nama item 
4. def update_jumlah_item(self): berfungsi untuk mengubah jumlah item
5. def update_harga_item(self): berfungsi untuk mengubah harga item
6. def delete_item(self): berfungsi untuk menghapus salah satu item
7. def reset_transaction(self): berfungsi untuk menghapus seluruh transaksi
8. def total_price(self): berfungsi untuk menghitung total harga
9. def tabel(self): berfungsi untuk membentuk tabel dengan mengimpor library tabulate

## Test Case
1. Setelah _run_ file maka akan muncul tampilan utama
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/0.%20Tampilan%20awal.png?raw=true)
2. fungsi add item
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/1.%20add%20item.png?raw=true)
3. fungsi update nama item
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/2.%20update%20nama.png?raw=true)
4. Setelah itu akan menjalankan fungsi update jumlah item
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/3.%20update%20harga.png?raw=true)
5. fungsi update harga item
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/4.%20update%20jumlah.png?raw=true)
6. fungsi delete item
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/5.%20delete%20item.png?raw=true)
7. fungsi reset transaction
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/6.%20reset%20transaction.png?raw=true)
8. fungsi check order
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/7.%20check%20order.png?raw=true)
9. fungsi total price
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/8.%20total%20price.png?raw=true)
10. fungsi keluar
![alt text](https://github.com/farhans10/Python-Pacmann/blob/master/img/9.%20keluar.png?raw=true)

## Conclusion
Project ini merupakan project sederhana sehingga masih perlu banyak perbaikan dan pengembangan lebih lanjut. Sarannya adalah dapat dipisah agar menjadi modular code

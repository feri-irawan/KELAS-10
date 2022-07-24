# Searching, Sorting, Stack dan Queue

Materi mengenai Searching, Sorting, Stack dan Queue.

## Pencarian (Searching)

Searching adalah sebuah metode pencarian guna menemukan data/informasi yang sedang dicari di dalam sebuah kumpulan data yang memiliki type data sama. Pencarian diperlukan untuk mendapatkan informasi/data dari kumpulan data yang belum diketahui.

```mermaid
stateDiagram-v2

Pengguna --> Kata_Kunci

Kata_Kunci --> Database: Cari data berdasarkan kata kunci yang dimasukkan.

Database --> NO: Jika data tidak ditemukan.
Database --> YES: Jika data ditemukan.
    
NO --> Hasil: Tampilkan teks "Data tidak ditemukan."
YES --> Data: Data 1, 2, 3 dan lainnya.

Data --> Hasil: Tampilkan data yang ditemukan.
Hasil --> Pengguna: Menampilkan hasil.
```

## Pengurutan (Sorting)

Sorting adalah proses mengatur sekumpulan objek menurut aturan atau susunan tertentu. Urutan objek tersebut dapat menaik (ascending = dari data kecil ke data lebih besar) atau menurun (descending = dari data besar ke data lebih kecil).

Contoh diagram untuk pengurutan menaik (ascending):
```mermaid
flowchart LR
A(..., 5, 4, 3, 2, 1) --> B(Mengurutkan data secara ascending)
B --> C(1, 2, 3, 4, 5, ...)
```

Contoh diagram untuk pengurutan menurun (descending):
```mermaid
flowchart LR
A(1, 2, 3, 4, 5, ...) --> B(Mengurutkan data secara descending)
B --> C(..., 5, 4, 3, 2, 1)
```

## Tumpukan (Stack)

Stack itu adalah struktur data yang menggunakan paradigma LIFO (Last In First Out), di mana elemen yang terakhir masuk adalah yang pertama keluar.  Misalkan, kita mempunyai setoples kue, jika kita ingin mengambil/mengeluarkan kue tersebut, otomatis kue yang pertama kita ambil adalah kue yang berada diposisi paling atas (yang terakhir dimasukkan)

Diagram stack:
```mermaid
flowchart

A(Kue terkahir masuk)
B(Kue yang pertama keluar)

3[(Kue ke-3)]
2[(Kue ke-2)]
1[(Kue ke-1, yang keluar terakhir.)]

A --> 3
B --> 3
3 --> 2
2 --> 1
```

## Antrian (Queue)

Queue merupakan struktur data yang menggunakan paradigma FIFO (First In First Out), dimana yang elemen pertama masuk adalah elemen yang pertama keluar. Contohnya saat kita mengantri untuk membeli sesuatu di toko atau minimarket, jika kita yang pertama mengantri, maka kita yang pertama keluar.

Diagram queue:
```mermaid
flowchart

A(Orang yang pertama mengantri)
B(Orang yang pertama keluar)

3(Orang ke-1)
2(Orang ke-2)
1(Orang ke-3, yang keluar terakhir.)

A --> 3
B --> 3
3 --> 2
2 --> 1
```

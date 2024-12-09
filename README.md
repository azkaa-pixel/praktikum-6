# modul praktikum 6
# sub rutin / fungsi

Nama : ghefira azka fardani 

Kelas : TI.24.A5

NIM : 312410521

## praktikum 6

### - flowchart
![foto](https://github.com/azkaa-pixel/praktikum-6/blob/8d3b90e4e211933eedd10e27d57f77f02550cd32/praktikum%206.png)
### - code program
#### 1. Daftar Mahasiswa (Dictionary)
```phython
mahasiswa = {}
```
Di sini, ```mahasiswa``` adalah sebuah dictionary kosong yang akan menyimpan data mahasiswa, 
dengan nama mahasiswa sebagai key dan nilai mahasiswa sebagai value. Contoh format data yang akan disimpan:
```phython
mahasiswa = {"ghefira": "A", "fabio": "e"}
```
#### 2. Fungsi ```tambah()```
```phython
def tambah(nama, nilai):
    """Fungsi untuk menambah data mahasiswa."""
    if nama in mahasiswa:
        print(f"Mahasiswa dengan nama {nama} sudah ada.")
    else:
        mahasiswa[nama] = nilai
        print(f"Data mahasiswa {nama} berhasil ditambahkan.")
```
Fungsi ```tambah()``` digunakan untuk menambahkan data mahasiswa baru. Jika nama mahasiswa sudah ada dalam dictionary ```mahasiswa```, maka program akan menampilkan pesan bahwa data mahasiswa sudah ada.
Jika tidak, data baru (nama dan nilai) akan ditambahkan ke dalam dictionary.
#### 3. Fungsi ```ubah()```
```phython
def ubah(nama, nilai_baru):
    """Fungsi untuk mengubah data mahasiswa berdasarkan nama."""
    if nama in mahasiswa:
        mahasiswa[nama] = nilai_baru
        print(f"Data mahasiswa {nama} berhasil diubah menjadi {nilai_baru}.")
    else:
        print(f"Mahasiswa dengan nama {nama} tidak ditemukan.")
```
Fungsi ```ubah()``` digunakan untuk mengubah nilai mahasiswa yang sudah ada. 
Jika mahasiswa dengan nama yang diberikan ditemukan dalam dictionary, maka nilai mahasiswa akan diubah. Jika tidak ditemukan, akan muncul pesan kesalahan.
#### 4. Fungsi ```hapus()```
```phython
def hapus(nama):
    """Fungsi untuk menghapus data mahasiswa berdasarkan nama."""
    if nama in mahasiswa:
        del mahasiswa[nama]
        print(f"Data mahasiswa {nama} berhasil dihapus.")
    else:
        print(f"Mahasiswa dengan nama {nama} tidak ditemukan.")
```
Fungsi ```hapus()``` digunakan untuk menghapus data mahasiswa berdasarkan nama.
Jika mahasiswa dengan nama yang diberikan ada dalam dictionary, maka data akan dihapus. Jika tidak ditemukan, pesan kesalahan akan ditampilkan.
#### 5. Fungsi tampilkan()
```phython
def tampilkan():
    """Fungsi untuk menampilkan daftar nilai mahasiswa."""
    if not mahasiswa:
        print("Daftar mahasiswa kosong.")
    else:
        print("Daftar Mahasiswa:")
        for nama, nilai in mahasiswa.items():
            print(f"Nama: {nama}, Nilai: {nilai}")
```
Fungsi ```tampilkan()``` akan menampilkan semua data mahasiswa yang ada di dalam dictionary ```mahasiswa```. Jika tidak ada data mahasiswa (dictionary kosong), program akan memberi pesan bahwa daftar mahasiswa kosong.
Jika ada data, maka nama dan nilai mahasiswa akan ditampilkan satu per satu.
#### 6. Menu Interaksi Pengguna
```phython
while True:
    print("\nMenu:")
    print("1. Tambah Mahasiswa")
    print("2. Ubah Nilai Mahasiswa")
    print("3. Hapus Mahasiswa")
    print("4. Tampilkan Daftar Mahasiswa")
    print("5. Keluar")
```
Di sini, program menyediakan menu interaksi untuk pengguna, yang memungkinkan mereka memilih salah satu tindakan yang ingin dilakukan. Menu ini terdiri dari 5 pilihan:

1. Tambah Mahasiswa
2. Ubah Nilai Mahasiswa
3. Hapus Mahasiswa
4. Tampilkan Daftar Mahasiswa
5. Keluar (untuk keluar dari aplikasi)
#### 7. Mekanisme Pilihan Menu
```phython
pilihan = input("Pilih menu (1-5): ")
```
Pengguna diminta untuk memilih salah satu menu dengan memasukkan angka 1 hingga 5.
Berdasarkan pilihan tersebut, program akan menjalankan fungsi yang sesuai.
#### 8. Eksekusi Pilihan
```phython
Bergantung pada input pengguna, program akan memanggil fungsi yang sesuai:

Pilihan 1: Meminta nama dan nilai untuk ditambahkan ke daftar.
Pilihan 2: Meminta nama mahasiswa yang nilainya ingin diubah dan nilai baru.
Pilihan 3: Meminta nama mahasiswa yang ingin dihapus dari daftar.
Pilihan 4: Menampilkan semua data mahasiswa yang ada.
Pilihan 5: Keluar dari aplikasi dan mengucapkan terima kasih.
Jika pengguna memilih pilihan yang tidak valid, program akan meminta mereka untuk memilih lagi.
```
Bergantung pada input pengguna, program akan memanggil fungsi yang sesuai:

Pilihan 1: Meminta nama dan nilai untuk ditambahkan ke daftar.

Pilihan 2: Meminta nama mahasiswa yang nilainya ingin diubah dan nilai baru.

Pilihan 3: Meminta nama mahasiswa yang ingin dihapus dari daftar.

Pilihan 4: Menampilkan semua data mahasiswa yang ada.

Pilihan 5: Keluar dari aplikasi dan mengucapkan terima kasih.

Jika pengguna memilih pilihan yang tidak valid, program akan meminta mereka untuk memilih lagi.

#### - hasil
![foto](https://github.com/azkaa-pixel/praktikum-6/blob/a5c11e838f0b934adbd7a58d5deceaab4fa7c9ad/hasil%206.jpg)



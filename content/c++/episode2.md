---
title: "Episode 1 Membuat Program Pertama C++"
date: 2019-05-12T12:14:34+06:00
image: "images/blog/c++.jpg"
description: "Membuat Program Pertama C++."
author: "Fahriz"
type: "post"
---

Belajar Pemrograman C++: Mengenal Variabel dan Tipe Data
# C++

 
Inti dari sebuah program komputer adalah menerima input, melakukan pemrosesan, dan menghasilkan output.

Input, proses, dan output
Nilai input bisa kita dapatkan dari keyboard, file, kamera, mikrofon, dan sebagainya.

Sementara output dapat kita tampilkan ke monitor, cetak ke dokumen, atau ke dalam sebuah file.

Pada tahap pemrosesan, program membutuhkan bantuan variabel untuk menyimpan nilai sementara.

Sama seperti waktu kita berpikir, kita membutuhkan beberapa ingatan untuk memproses informasi.

Pada tutorial ini, saya akan bahas tuntas tentang cara penggunaan variabel dan tipe data dalam pemrograman C++.

Siap?

Mari kita mulai…

Apa itu Variabel dan Tipe Data?
Semua program komputer yang sedang berjalan akan menyimpan data sementara di dalam RAM (Random Access Memori).

Data-data yang tersimpan di dalam RAM memiliki alamat yang direpresentasikan dalam bilangan heksa desmial.

Bagaiaman cara program menyimpan nilai ke RAM?

Jawabannya dengan menggunakan variabel.

Semakin banyak variabel yang kamu buat semakin besar pula memori yang akan digunakan di dalam RAM.

Penyimpanan data di dalam RAM
Jadi dapat kita simpulkan…

Variabel adalah sebuah nama lokasi penyimpanan di dalam memori.

Sementara tipe data adalah jenis data yang akan disimpan di dalam variabel.

Macam-macam tipe data di C++ dapat dilihat dari tabel berikut.

| Nama                   | Tipe Data	Ukuran dalam Memori   | Rentang Nilai                       |
|----------------------- |---------------------------------|----------------------------------   |
| char	                  | 1byte	                          | -127 sampai 127 atau 0 sampai 255   |
| unsigned char	         | 1byte	                          | 0 sampai 255                        |
| signed char	           | 1byte                           | -127 sampai 127                     |
| int	                   | 4bytes	                         | -2147483648 sampai 2147483647       |
| unsigned int	          | 4bytes	                         | 0 sampai 4294967295                 |
| signed int	            | 4bytes                          | -2147483648 sampai 2147483647       |
| short int	             | 2bytes	                         | -32768 sampai 32767                 |
| unsigned short int	    | Range                           | 0 sampai 65,535                     |
| signed short int	      | Range	                          | -32768 sampai 32767                 |
| long int	              | 4bytes                          | -2,147,483,648 sampai 2,147,483,647 |
| signed long int        |	4bytes                          | same as long int                    |
| unsigned long int      |	4bytes                          | 0 sampai 4,294,967,295              |
| float	                 | 4bytes	                         | +/- 3.4e +/- 38 (~7 digits)         |
| double	                | 8bytes                          | 	+/- 1.7e +/- 308 (~15 digits)      |
| long double	           | 8bytes	                         | +/- 1.7e +/- 308 (~15 digits)       |
| wchar_t                |	2 or 4 bytes	                   | 1 wide character                    |
| boolean	               | 4bytes	                         | true atau false                     |

**Cara Membuat Variabel di C++**
Pembuatan variabel atau deklarasi variabel di C++ dapat kita lakukan seperti berikut ini:
```C++
string nama;
int umur;
char jenis_kelamin;
```
>Tipe datanya ditulis terlebih dahulu, lalu diikuti dengan nama variabelnya.

Variabel-variabel di atas akan menyimpan nilai null (kosong), karena belum kita isi.

Kita juga dapat membuat variabel dengan mengisinya langsung.

Contoh:
```C++
string nama = "Fahriz Coding";
float tinggi = 169.43;
Untuk lebih jelasnya, mari kita coba praktekkan dalam program.
```

>Membuat Porgram C++ dengan Variabel dan Tipe Data
>Silahkan buat sebuah file baru bernama biodata.cpp, kemudian isi dengan kode berikut:

```C++
#include <iostream>

using namespace std;

int main(){
 
  // deklarasi tipe data variabel
  string nama;
  int umur;
  char jenis_kelamin;
 
  // --- proses input ---
  cout << "Siapakah namamu?" << endl;
  cout << "jawab: ";
  // menyimpan data ke variabel
  getline(cin,nama);
 
  cout << "Berapa umurmu?" << endl;
  cout << "jawab: ";
  // menyimpan data ke variabel
  cin >> umur;
 
  cout << "Jenis kelamin [L/P]: ";
  // menyimpan data ke variabel
  cin >> jenis_kelamin;
 
  // --- proses output ---
  cout << "Salam kenal, " << nama << " Sekarang engkau berusia ";
  cout << umur << " dan kau berjenis kelamin "<< jenis_kelamin;
 
  return 0;

}
```

Setelah itu lakukan kompilasi dan eksekusi programnya.

Kompilasi dan eksekusi Program C++
Mudah bukan?

**Bedah Kode : **

Pertama dimulai dari membuat variabel.

```C++
string nama;
int umur;
char jenis_kelamin;
```

Pada baris kode tersebut, kita membuat tiga buah variabel dengan tipe data yang berbeda-beda.

Lalu kita mengisi nilainya berdasarkan input yang diberikan dari keyboard dengan perintah cin.
```C++
cin >> umur;
cin >> jenis_kelamin;
```
>Khusus untuk tipe data string, kita menggunakan fungsi getline() untuk mengambil satu baris nilai yang diinputkan.
```C++
getline(cin,nama);
```
Terakhir kita menampilkan isi variabelnya dengan perintah cout.

Mengubah Nama Tipe Data
Kita bisa mengubah nama tipe data sendiri dengan perintah typedef.

Membuat tipe data baru di C++

>Contohnya:

>typedef int angka; 
>Artinya, tipe data int (integer) akan kita buat namanya menjadi angka.

Lalu, untuk menggunakannya kita bisa tulis seperti ini:

angka umur;
Apa Selanjutnya?

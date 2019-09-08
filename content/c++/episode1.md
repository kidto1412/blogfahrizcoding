---
title: "PHP part 1 : Pengenalan PHP"
date: 2019-05-12T12:14:34+06:00
image: "images/blog/c++.jpg"
description: "Pengenalan PHP."
author: "Fahriz"
type: "post"
---

Ada banyak alat yang bisa kita gunakan untuk belajar pemrograman C++ .

Bisa menggunakan Borland c++, Codeblocks, Codelite, Dev c++, dan sebagainya.

Namun, yang akan kita bahas di sini adalah menggunakan teks editor Devc++
kalian bisa mendownload disini : https://dev-c.soft32.com/

Pengertian Bahasa Pemrograman C++
Bahasa pemrograman C++ merupakan bahasa pengembangan dari bahasa C.

Apa bedanya C++ dengan C?

C++ memiliki fitur yang lebih banyak dari C.

Contohnya:

Pada bahasa C, kita tidak bisa membuat class sedangkan pada C++ kita bisa membuatnya.

Alat-alat untuk Membuat Program C++
Sebenarny ada dua alat yang harus kita persiapkan:

Teks Editor: sebagai tempat menulis kode.
Kompilator g++: Program yang menerjemahkan bahasa C++ menjadi bahasa mesin (executable).

Membuat Program C++ Pertama
Baik, sekarang kita akan coba membuat program Hello World.

>Pertama
kita buka dev c++ klik new project => console aplication
image: "images/blog/new project konsole.jpg"


kemudian ketik kode berikut:
 image: "images/blog/source.jpg"
 #include <iostream>
 using namespace std;

 int main(){
    cout << "Hello World!" << endl;
   return 0;
 }

Lalu klik Execute compile and run
image: "images/blog/execute.jpg"

maka hasilnya akan seperti ini:
image: "images/blog/hasil.jpg"

 



Bedah Kode
Waktunya saya menjelaskan arti dan maksud dari kode program di atas.

Pertama dimulai dari:

#include <iostream>
Maksud dari kode di atas adalah mendeklarasikan fungsi apa saja yang akan kita gunakan dalam program.

Contohnya:

Karena kita membutuhkan fungsi cout untuk menampilkan teks ke layar, maka kita harus mengimpor fungsi tersebut dari <iostream>.

Fungsi cout berada dalam namespace std.

Maka kita membutuhkan kode berikut:

using namespace std;
Jika tanpa itu, kita akan menuliskan perintah cout lengkap dengan namespace-nya:

std::cout << "Hello world";
Setelah itu, kita membuat fungsi main.

Fungsi main adalah fungsi utama di dalam program C++.

Fungsi ini akan dieksekusi pertamakali setiap kali program dijalankan.

int main(){
    cout << "Hello World!" << endl;
    return 0;
}
Kita harus menuliskan perintah atau fungsi di dalam fungsi main agar dapat dieksekusi.

Sebagai contoh, kita memberikan perintah:

cout << "Hello World!" << endl;
Perintah cout adalah perintah untuk menampilkan teks ke layar.

Tunggu dulu, apa itu endl?

endl (endline) fungsinya untuk membuat baris baru.

Contoh:

cout << "Hello" << endl;
cout << "World!" << endl;
Akan menghasilkan output:

Hello
World!
Sedangkan tanpa endl:

cout << "Hello";
cout << "World!";
akan menghasilkan:

Hello World!
Lalu, terakhir ada perintah return 0 apa artinya?

Karena fungsi main yang kita buat memiliki kembalikan berupa nilai integer:

int main(){
    ...
}
Maka harus ada nilai kembalian berupa integer. Nol (0) adalah salah satu nilai intege

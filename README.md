# javascript-SL

https://www.youtube.com/watch?v=qwL6ISjbaaE

# SYNC / BLOCKING ? 
Program javascript by default akan dieksekusi baris per baris. 

By default proses di JavaScript akan dieksekusi secara Sync, artinya baris selanjutnya akan dieksekusi setelah baris sebelumnya selesai dikerjakan. 

![image](https://github.com/affodilajF/javascript-SL/assets/130672181/017d8e31-4a2d-4db8-83fd-a38e246add6e)


# ASYNC / NON-BLOCKING ? 
Pada proses async, js tidak akan menunggu proses tsb selesai, melainkan akan melanjutkan ke baris selanjutnya tanpa harus menunggu proses async selesai. 

Get Product by Id lama nih misalnya, akan dialihkan ke async proses, sementara main thread akan berjalan sequential. Kalo proses get productnya udah selesai, baru balik ke main thread (menggunakan callback). 

![image](https://github.com/affodilajF/javascript-SL/assets/130672181/5eea2348-dc57-48ba-aa7e-ff704a037531)

# CALLBACK 
Adalah mekanisme untuk memanggil kembali kode yang ada di program dari proses Async. 

Callback biasanya dibuat dalam bentuk function as parameter, dan parameter function tersebut akan dieksekusi saat proses Async selesai. 

# ASYNC METHOD
Ada banyak. Contohnya : 
- setTimeout(callback, timelnMilis) => digunakan untuk menjalankan proses Async sekali dalam waktu tertentu. Callback akan dipanggil setelah waktu timenMilis habis.
- setInterval (callback, timelnMilis) => digunakan untuk menjalankan proses Async secara periodik dalam waktu tertentu. Callback akan dipanggil berkali-kali dalam interval timelnMilis.

![image](https://github.com/affodilajF/javascript-SL/assets/130672181/9a63a2dd-858a-4893-a30d-eea16ea90af6)

![image](https://github.com/affodilajF/javascript-SL/assets/130672181/33769001-3659-4b11-8b83-816507aad56a)

# AJAX (async js and xml)
Ajax digunakan untuk menggambil atau mengirim data ke URL lain (url di server) 
.
Cara bikin? pake kelas XMLHttpRequest. 

cara kerja => mengirim req menerima req ke server.
![image](https://github.com/affodilajF/javascript-SL/assets/130672181/d9981888-a436-4d20-8b42-22a56b501c1f)

![image](https://github.com/affodilajF/javascript-SL/assets/130672181/06ed224b-18bb-4cf3-adc5-bf83d3c169eb)

### Menerima Data di Ajax 
Ajax digunakan untuk mengirim&/menerima data dari server. 

Tiap request ajax, biasanya kita ingin mendapatkan informasi response yang diberikan server. 

Kita tidak bisa langsung menggambil response AJAX karena proses AJAX adalah Async, sehingga kita perlu menunggu sampai proses Async nya selesai. 

Untuk mendapatkan informasi AJAX, kita bisa menggunakan AJAX Callback, yang akan dieksekusi setelah proses AJAX selesai. 

Untuk menambahkan AJAX Callback, kita bisa tampahkan pada event listener / event load. 

Dan untuk menggambil datanya dari server, kita bisa menggunakan property responseText.

![image](https://github.com/affodilajF/javascript-SL/assets/130672181/b1b36eaf-ed4a-471d-94ed-2e76d0864262)



































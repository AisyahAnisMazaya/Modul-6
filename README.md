1. Kode di atas adalah program Go yang digunakan untuk menghitung dan mencetak deret Fibonacci hingga suatu bilangan tertentu.
package main: Menyatakan bahwa ini adalah program utama.
import "fmt": Mengimpor paket fmt untuk melakukan input/output.
func fibonacci(n int) int: Fungsi rekursif yang menghitung nilai Fibonacci ke-n.
func main(): Fungsi utama tempat eksekusi program dimulai.
var n int: Mendeklarasikan variabel n untuk menyimpan jumlah deret Fibonacci yang diinginkan.
fmt.Print("Masukkan jumlah deret Fibonacci: ") : Mencetak prompt untuk meminta input pengguna.
fmt.Scan(&n): Membaca input pengguna dan menyimpannya ke variabel n.
fmt.Printf("Deret Fibonacci untuk %d angka adalah:\n", n): Mencetak pesan yang menunjukkan jumlah deret Fibonacci yang akan ditampilkan.
for i := 0; i < n; i++: Looping untuk mencetak setiap nilai Fibonacci dari 0 hingga n-1.
fmt.Printf("%d ", fibonacci(i)): Mencetak nilai Fibonacci ke-i.
Cara Kerja:
Program meminta pengguna untuk memasukkan jumlah deret Fibonacci yang diinginkan.
Nilai yang dimasukkan disimpan dalam variabel n.
Program kemudian memanggil fungsi fibonacci secara berulang untuk menghitung setiap nilai Fibonacci hingga n.
Setiap nilai Fibonacci yang dihitung akan dicetak ke layar.

2. Kode di atas adalah program Go yang digunakan untuk mencetak pola bintang berbentuk segitiga siku-siku.
package main: Menyatakan bahwa ini adalah program utama.
import "fmt": Mengimpor paket fmt untuk melakukan input/output.
func printStars(baris, n int): Fungsi yang digunakan untuk mencetak bintang.
baris: Menunjukkan baris saat ini yang sedang dicetak.
n: Menunjukkan jumlah total baris yang diinginkan.
if baris > n: Jika baris yang sedang dicetak melebihi jumlah baris yang diinginkan, maka fungsi akan berhenti.
for i := 1; i <= baris; i++: Looping untuk mencetak bintang sebanyak nilai baris.
fmt.Print("*"): Mencetak satu karakter bintang.
fmt.Println(): Memindahkan kursor ke baris berikutnya.
printStars(baris+1, n): Memanggil fungsi printStars secara rekursif untuk mencetak baris berikutnya.
func main(): Fungsi utama tempat eksekusi program dimulai.
var n int: Mendeklarasikan variabel n untuk menyimpan jumlah baris yang diinginkan.
fmt.Print("Masukkan jumlah baris: ") : Mencetak prompt untuk meminta input pengguna.
fmt.Scan(&n): Membaca input pengguna dan menyimpannya ke variabel n.
printStars(1, n): Memanggil fungsi printStars untuk memulai mencetak pola bintang dari baris pertama.
Cara Kerja:
Program meminta pengguna untuk memasukkan jumlah baris yang diinginkan.
Nilai yang dimasukkan disimpan dalam variabel n.
Program kemudian memanggil fungsi printStars dengan nilai awal baris 1 dan jumlah baris n.
Fungsi printStars akan mencetak bintang sebanyak nilai baris saat ini, kemudian memanggil dirinya sendiri secara rekursif untuk mencetak baris berikutnya. Proses ini terus berulang hingga baris yang dicetak melebihi jumlah baris yang diinginkan.

3. Kode di atas adalah program Go yang dirancang untuk mencari dan mencetak faktor-faktor pembagi dari sebuah bilangan bulat positif. Namun, ada beberapa kejanggalan dalam kode ini yang perlu diperhatikan.
Fungsi faktor:
Parameter: Fungsi ini menerima dua parameter integer, yaitu n yang mewakili bilangan yang akan dicari faktornya, dan i yang merupakan pembagi yang sedang diuji.
Kondisi berhenti: Jika n kurang dari atau sama dengan 1, maka fungsi akan berhenti secara rekursif.
Menemukan faktor: Jika n habis dibagi i (artinya i adalah faktor dari n), maka nilai i akan dicetak.
Panggilan rekursif: Fungsi akan memanggil dirinya sendiri dengan nilai i yang ditambah 1, sehingga secara bertahap semua bilangan dari 1 hingga n akan diuji sebagai pembagi.
Fungsi main:
Meminta input: Program meminta pengguna untuk memasukkan sebuah bilangan.
Memanggil fungsi faktor: Fungsi faktor dipanggil dengan parameter n (bilangan yang dimasukkan pengguna) dan i dengan nilai awal 1.
Mencetak hasil: Hasil dari fungsi faktor (yaitu faktor-faktor pembagi) akan dicetak di layar.

4. Penjelasan Kode:
Kode di atas adalah program Go yang menggunakan konsep rekursi untuk mencetak suatu urutan bilangan secara khusus.
Fungsi rekursifSequence:
Parameter: Fungsi ini menerima satu parameter integer n yang menentukan batas atas urutan bilangan yang akan dicetak.
Kondisi dasar: Jika n sama dengan 1, maka fungsi akan mencetak angka 1 dan langsung berhenti (return). Ini adalah kasus dasar dari rekursi.
Cetak nilai: Fungsi akan mencetak nilai n terlebih dahulu.
Panggilan rekursif: Kemudian, fungsi akan memanggil dirinya sendiri dengan nilai n-1, yang berarti akan mencetak urutan bilangan yang lebih kecil secara rekursif.
Cetak nilai lagi: Setelah panggilan rekursif selesai, fungsi akan mencetak nilai n sekali lagi.
Fungsi main:
Meminta input: Program meminta pengguna untuk memasukkan sebuah bilangan.
Memanggil fungsi rekursif: Fungsi rekursifSequence dipanggil dengan nilai n yang dimasukkan pengguna, sehingga urutan bilangan akan dicetak mulai dari n hingga 1 dan kemudian kembali ke n.
Cara Kerja:
Input: Pengguna memasukkan sebuah bilangan n.
Panggilan awal: Fungsi rekursifSequence dipanggil dengan nilai n.
Cetak nilai pertama: Nilai n dicetak.
Panggilan rekursif: Fungsi memanggil dirinya sendiri dengan n-1.
Ulangi langkah 3 dan 4: Langkah 3 dan 4 diulang hingga n menjadi 1.
Cetak nilai terakhir: Setelah semua panggilan rekursif selesai, nilai n awal dicetak lagi.

5. Penjelasan Kode:
Kode di atas adalah program Go yang dirancang untuk mencetak bilangan ganjil dari n hingga 1 secara rekursif.
Fungsi bilanganGanjil:
Parameter: Fungsi ini menerima satu parameter integer n yang merupakan batas atas bilangan yang akan dicetak.
Kondisi berhenti: Jika n kurang dari atau sama dengan 1, maka fungsi akan berhenti secara rekursif.
Cek bilangan ganjil: Jika n dibagi 2 sisanya 1 (artinya n adalah bilangan ganjil), maka n akan dicetak.
Panggilan rekursif: Fungsi akan memanggil dirinya sendiri dengan nilai n-2, sehingga akan melompati bilangan genap dan hanya mencetak bilangan ganjil.
Fungsi main:
Meminta input: Program meminta pengguna untuk memasukkan sebuah bilangan n.
Cek bilangan genap atau ganjil: Program memeriksa apakah n adalah bilangan ganjil atau genap.
Panggilan fungsi:
Jika n ganjil, fungsi bilanganGanjil dipanggil dengan nilai n.
Jika n genap, fungsi bilanganGanjil dipanggil dengan nilai n-1 agar dimulai dari bilangan ganjil terdekat.
Cara Kerja:
Input: Pengguna memasukkan sebuah bilangan n.
Cek genap/ganjil: Program memeriksa apakah n genap atau ganjil.
Panggilan rekursif: Fungsi bilanganGanjil dipanggil dengan nilai yang sesuai.
Cetak bilangan ganjil: Fungsi akan mencetak bilangan ganjil secara rekursif, dimulai dari n atau n-1 (tergantung apakah n genap atau ganjil).
Contoh Output:
Jika pengguna memasukkan nilai 7, maka output yang dihasilkan adalah:
7 5 3 1
Pola Output:
Program akan mencetak bilangan ganjil dari n hingga 1 secara menurun.
Konsep Penting:
Rekursi: Fungsi memanggil dirinya sendiri secara berulang hingga mencapai kondisi dasar.
Bilangan ganjil: Program hanya mencetak bilangan yang habis dibagi 2 sisanya 1.
Penjelasan Singkat:
Kode ini menggunakan rekursi untuk mencetak bilangan ganjil dari n hingga 1. Dengan memeriksa setiap bilangan apakah ganjil atau tidak, dan memanggil fungsi secara rekursif untuk bilangan yang lebih kecil, program ini menghasilkan urutan bilangan ganjil.

6. Penjelasan Kode:
Kode di atas adalah program Go yang digunakan untuk menghitung nilai pangkat dari suatu bilangan.
Fungsi pangkat:
Parameter: Fungsi ini menerima dua parameter integer, yaitu x yang merupakan bilangan dasar dan y yang merupakan pangkat.
Kondisi dasar: Jika y sama dengan 0, maka fungsi akan mengembalikan nilai 1 (karena setiap bilangan pangkat 0 adalah 1).
Panggilan rekursif: Jika y tidak sama dengan 0, fungsi akan mengembalikan hasil perkalian antara x dengan hasil pemanggilan fungsi pangkat dengan parameter x dan y-1. Ini adalah inti dari perhitungan pangkat secara rekursif.
Fungsi main:
Meminta input: Program meminta pengguna untuk memasukkan nilai x sebagai bilangan dasar dan y sebagai pangkat.
Memanggil fungsi pangkat: Fungsi pangkat dipanggil dengan nilai x dan y yang telah diinputkan pengguna.
Mencetak hasil: Hasil dari pemanggilan fungsi pangkat akan disimpan dalam variabel hasil dan kemudian dicetak ke layar.
Cara Kerja:
Input: Pengguna memasukkan nilai x dan y.
Panggilan rekursif: Fungsi pangkat dipanggil dengan nilai x dan y.
Perhitungan: Fungsi pangkat akan terus memanggil dirinya sendiri dengan nilai y yang semakin kecil hingga mencapai kondisi dasar (y == 0).
Hasil: Setelah mencapai kondisi dasar, hasil perhitungan akan dikembalikan ke pemanggilan fungsi sebelumnya, dan seterusnya hingga mencapai panggilan awal.
Cetak hasil: Hasil akhir dari perhitungan akan dicetak ke layar.


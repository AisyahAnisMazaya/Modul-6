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


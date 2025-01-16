# Belajar Golang Basic

Panduan ini dirancang untuk membantu Anda memulai belajar bahasa pemrograman **Go (Golang)**. Go adalah bahasa pemrograman yang cepat, efisien, dan dirancang untuk aplikasi modern.

## Prasyarat

Sebelum memulai, pastikan Anda memiliki:
- Dasar-dasar pemrograman.
- Akses ke terminal atau command prompt.
- Go sudah terinstal di komputer Anda. Jika belum, ikuti [panduan instalasi Go](https://go.dev/doc/install).

## Instalasi Go

1. Unduh installer Go dari [halaman resmi Go](https://go.dev/dl/).
2. Ikuti petunjuk instalasi sesuai sistem operasi Anda.
3. Verifikasi instalasi dengan menjalankan perintah berikut di terminal:
   ```bash
   go version
   ```
   Anda akan melihat output seperti:
   ```
   go version go1.xx.x <os>/<arch>
   ```

## Struktur Dasar Program Go

Setiap program Go dimulai dengan fungsi `main`. Berikut adalah contoh program dasar:

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello, World!")
}
```

### Penjelasan:
- **`package main`**: Menentukan paket utama yang dieksekusi.
- **`import "fmt"`**: Mengimpor paket standar untuk output.
- **`func main()`**: Fungsi utama tempat program dimulai.

## Menjalankan Program Go

1. Buat file baru bernama `main.go`.
2. Salin kode di atas ke dalam file tersebut.
3. Jalankan perintah berikut untuk mengeksekusi program:
   ```bash
   go run main.go
   ```
   Output:
   ```
   Hello, World!
   ```

## Konsep Dasar Golang

### 1. Variabel

Deklarasi variabel di Go:
```go
package main

import "fmt"

func main() {
    var name string = "John"
    age := 25

    fmt.Println("Name:", name)
    fmt.Println("Age:", age)
}
```

### 2. Kondisional

Contoh penggunaan `if` dan `else`:
```go
package main

import "fmt"

func main() {
    age := 20

    if age >= 18 {
        fmt.Println("Dewasa")
    } else {
        fmt.Println("Belum Dewasa")
    }
}
```

### 3. Perulangan

Go mendukung perulangan menggunakan `for`:
```go
package main

import "fmt"

func main() {
    for i := 1; i <= 5; i++ {
        fmt.Println(i)
    }
}
```

### 4. Fungsi

Deklarasi dan pemanggilan fungsi:
```go
package main

import "fmt"

func greet(name string) string {
    return "Hello, " + name
}

func main() {
    message := greet("Alice")
    fmt.Println(message)
}
```

## Tools Pendukung

- **Go Modules**: Untuk mengelola dependensi proyek.
  ```bash
  go mod init <nama-proyek>
  ```
- **`go fmt`**: Untuk memformat kode Go secara otomatis.
  ```bash
  go fmt <file.go>
  ```
- **`go build`**: Untuk membangun file biner dari kode Go.
  ```bash
  go build main.go
  ```

## Sumber Belajar Tambahan

- [Dokumentasi Resmi Go](https://go.dev/doc/)
- [Tutorial Go by Golang.org](https://tour.golang.org/)
- [Go Playground](https://play.golang.org/): Untuk mencoba kode Go langsung di browser.


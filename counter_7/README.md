**Shayna Putri Fitria - 2106703084**

# **Tugas 7 - Elemen Dasar Flutter**

## 1. Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.

### **Stateless Widget**

- Widget yang stateless tidak berubah atau immutable, 
- Hanya memiliki final properties yang didefinisikan saat construction

### **Stateful Widget**

- Widget yang stateful dapat berubah ketika ada perubahan eksternal atau ketika ada user yang berinteraksi, bersifat mutable
- Contoh: Checkbox, Radio, Slider

## 2. Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.

- Menggunakan widget Text untuk menampilkan counter dan menunjukkan apakah dia GANJIL atau GENAP
- Menggunakan widget FloatingActionButton sebagai event untuk menambah atau mengurangi counter yang akan di pressed oleh user

## 3. Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.

- Fungsi setState hanya dapat digunakan pada stateful widget
- setState() berfungsi sebagai penanda bahwa ada event yang sedang menimbulkan perubahan pada State yang juga akan merubah widget, maka aplikasi akan memuat ulang program dan nilai/ data pada widget akan berubah
  
## 4. Jelaskan perbedaan antara const dengan final.

### **Final**
- Variabel yang Final akan meletakkan kata 'final' sebelum variabelnya
- Nilai variabel Final hanya akan diinisialisasi di awal atau pertama kali didefinisikan
- Akan diketahui saat run time, sehingga variabel boleh sudah atau belum memiliki nilai variabel
- Dapat digunakan untuk deklarasi variabel yang ingin bersifat immutable

### **Const**
- Variabel yang Const akan meletakkan kata 'const' sebelum variabelnya
- Dapat digunakan untuk deklarasi variabel yang ingin bersifat mutable dan nilainya bersifat konstan
- Akan diketahui saat compile time, sehingga variabel harus memiliki value atau didefinisikan secara langsung

## 5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
- **Membuat sebuah program Flutter baru dengan nama counter_7**: Menjalankan command 'flutter create' pada command prompt
- **Mengubah tampilan program menjadi seperti berikut**: Membuat 2 FloatingActionButton untuk tombol increment (+) dan decrement (-) yang akan dihubungkan dengan function atau event listenernya masing-masing
- **Tombol + menambahkan angka sebanyak satu satuan**: Dilakukan dengan membuat function increment counter yang di trigger oleh FloatingActionButton (+)
- **Tombol - mengurangi angka sebanyak satu satuan. Apabila counter bernilai 0, maka tombol - tidak memiliki efek apapun pada counter**: Dilakukan dengan membuat function decrement yang di trigger oleh FloatingActionButton (-)
- **Apabila counter bernilai ganjil, maka teks indikator berubah menjadi "GANJIL" dengan warna biru**: Membuat if conditional dalam function increment & decrement, jika remainder dari pembagian 2 adalah 1, maka akan bertuliskan "GANJIL" dan berwarna biru
- **Apabila counter bernilai genap, maka teks indikator berubah menjadi "GENAP" dengan warna merah**: Membuat if conditional dalam function increment & decrement, jika remainder dari pembagian 2 adalah 0, maka akan bertuliskan "GENAP" dan berwarna merah
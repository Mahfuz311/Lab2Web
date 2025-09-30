# Praktikum Web 2 – CSS Dasar

Nama : Mahfuz Fauzi

NIM : 312410412

Kelas : TI.24.A3

## Langkah-langkah Praktikum

### 1. Membuat dokumen HTML

```
Code HTML :
```
<img src="https://github.com/Mahfuz311/Lab2Web/blob/0abe68e8ff0c5eb83462341337914c1929e2bcc1/screenshot/1%20vscode.png">

**Output/tampilan Websitenya:**

<img src="https://github.com/Mahfuz311/Lab2Web/blob/0abe68e8ff0c5eb83462341337914c1929e2bcc1/screenshot/1%20web.png">

---

### 2. Mendeklarasikan CSS Internal

Menambahkan deklarasi CSS internal pada bagian head dokumen

```
Code HTML :
```
<img src="https://github.com/Mahfuz311/Lab2Web/blob/0abe68e8ff0c5eb83462341337914c1929e2bcc1/screenshot/2%20vscode.png">

**Outputnya:**

<img src="https://github.com/Mahfuz311/Lab2Web/blob/0abe68e8ff0c5eb83462341337914c1929e2bcc1/screenshot/2%20web.png">

---

### 3. Menambahkan Inline CSS

Menambahkan deklarasi inline CSS pada tag **`<p>`** seperti berikut.

```
Code HTML :
```
<img src="https://github.com/Mahfuz311/Lab2Web/blob/0abe68e8ff0c5eb83462341337914c1929e2bcc1/screenshot/3%20vscode.png">

**Outputnya:**

<img src="https://github.com/Mahfuz311/Lab2Web/blob/0abe68e8ff0c5eb83462341337914c1929e2bcc1/screenshot/3%20web.png">

---

### 4. Membuat CSS Eksternal

Buat file baru dengan nama **`style_eksternal.css`** dan deklarasi CSS seperti berikut.

```
Code HTML :
```

<img src="https://github.com/Mahfuz311/Lab2Web/blob/ddae10299d13284e54fb1b73e02b9c3ffb98eba9/screenshot/4.0%20vscode.png">

Kemudian menambahkan tag **`<link>`** untuk merujuk file CSS yang sudah dibuat pada bagian **`<head>`**

<img src="https://github.com/Mahfuz311/Lab2Web/blob/511ee6ce3e94e7e96b2e19b998759a8119d78c88/screenshot/4.1%20vscode.png">

**Output/tampilan Websitenya:**

<img src="https://github.com/Mahfuz311/Lab2Web/blob/027c0e6b133e2c6c7e2139ecf44dd0a64583a644/screenshot/4.0%20web.png">

---

### 5. Menambahkan CSS Selector

Menambahkan CSS selector menggunakan ID dan Class Selector. Pada file **`style_eksternal.css`**

```
Code HTML :
```
<img src="https://github.com/Mahfuz311/Lab2Web/blob/ddae10299d13284e54fb1b73e02b9c3ffb98eba9/screenshot/4%20vscode.png">

**Output/tampilan Websitenya:**

<img src="https://github.com/Mahfuz311/Lab2Web/blob/027c0e6b133e2c6c7e2139ecf44dd0a64583a644/screenshot/4%20web.png">

---

## Pertanyaan dan Tugas Praktikum

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.

   **Jawaban:**
   Misalnya Saya punya kode CSS awal:
   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/5.1%20vscode.png">
   
   Kemudian Saya ubah dan tambahkan propertinya:

   ```css
   h1 {
     color: blue;
     font-size: 30px;
     text-align: center;
     padding: 10px;
   }
   ```
   
   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/5%20vscode.png">

   **Outputnya:**

   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/5%20web.png">

   Hasilnya, teks `<h1>` akan tampil biru, berukuran `30px`, di tengah halaman, dengan `background` kuning dam ada `padding`.

   ---

2. Apa perbedaan pendeklarasian CSS elemen `h1 {…}` dengan `#intro h1 {…}`? berikan penjelasannya!

   **Jawaban:**

   - `h1 {...}`
     Selector elemen. Artinya semua elemen `<h1>` di halaman web akan mendapatkan style tersebut.
   - `#intro h1 {...}`
     Selector ID + elemen. Artinya hanya `<h1>` yang berada di dalam elemen dengan `id="intro"` saja yang terkena style.
   Contoh:

   ```
   HTML
   ```

   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/6.1%20vscode.png">

   ```
   CSS
   ```

   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/6.2%20vscode.png">

   **Hasilnya:**

   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/6%20web.png">

   - "Judul" berwarna merah
   - "Judul di Intro" berwarna biru
   ---

3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

   **Jawaban:**

   Urutan prioritas deklarasi CSS (eksternal, internal, inline)
   - Eksternal CSS = ditulis do file `.css` terpisah.
   - Internal CSS = ditulis di `<style>...</style>` dalam file HTML.
   - Inline CSS = ditulis langsung di atribut elemen HTML (`<h1 style="color:green">`).
   Urutan prioritasnya:
   1. Inline CSS = prioritas tertinggi.
   2. Internal CSS
   3. Eksternal CSS = prioritas paling rendah.
   
   **Screenshot Vscode & Browser**

   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/7%20vscode.png">
   
   <br>
   
   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/7%20web.png">
   
   Hasil di browser: hijau, karena inline CSS lebih kuat.

   ---

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! (`<p id="paragraf-1" class="text-paragraf">`)

   **Jawaban:**

   Perbedaan ID dan Class (jika keduanya ada pada elemen yang sama)

   - ID (`#id`) = lebih spesifik daripada Class (`.class`).
   - Jika elemen punya ID dan Class sekaligus, maka CSS ID akan menang jika keduanya memberi style berbeda pada properti yang sama.
   Contoh:
   `HTML`
   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/8.1%20vscode.png">

   `CSS`
   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/8.2%20vscode.png">

   **Hasilnya**

   <img src="https://github.com/Mahfuz311/Lab2Web/blob/9ae399a0b9c566aceb45d4ada315678485f3a48a/screenshot/8%20web.png">

   Hasil dari browser: teks paragraf berwarna biru, karena ID lebih kuat daripada Class.

   

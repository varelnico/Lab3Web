# Praktikum 3: CSS Dasar - Lab3Web

Praktikum mata kuliah **Pemrograman Web** memahami konsep dasar CSS, aturan penulisan, selector, serta penerapan CSS (Internal, Eksternal, dan Inline) pada dokumen HTML.

## Identitas Mahasiswa
Nama : Varel Nico Ramadhan
NIM : 312510156
Kelas : I251B  
Mata Kuliah : Pemrograman Web

## 1. Langkah-Langkah Praktikum & Implementasi

### Langkah 1: Membuat Dokumen HTML Dasar 
Membuat struktur dasar dokumen HTML dengan menyertakan navigasi, elemen header, serta pembungkus dengan ID dan Class selector.

<img width="1920" height="1080" alt="code 1" src="https://github.com/user-attachments/assets/85598961-29e4-412e-86b6-8ab821f2c3c3" />
<img width="1920" height="1080" alt="hasil 1" src="https://github.com/user-attachments/assets/6e92ffc0-5860-4e55-a37e-cc56ac5baf5b" />




### Langkah 2: Mendeklarasikan CSS Internal
Menambahkan tag `<style>` pada bagian `<head>` dokumen untuk mengatur gaya dasar seperti font, padding, border, dan warna teks pada elemen `header` dan `h1`.

<img width="1920" height="1080" alt="code 2" src="https://github.com/user-attachments/assets/92bc69ac-e150-4957-8f3d-02657f7a68f9" />
<img width="1920" height="1080" alt="hasil 2" src="https://github.com/user-attachments/assets/95315443-e222-4e2a-aea7-5fbc55eae06d" />



### Langkah 3: Menambahkan Inline CSS
Menambahkan deklarasi inline CSS langsung pada tag paragraf `<p>` untuk mengubah gaya pada baris tertentu secara spesifik.

<img width="1920" height="1080" alt="code 3" src="https://github.com/user-attachments/assets/8b05deed-38b1-41b7-bda9-3d10087f29db" />
<img width="1920" height="1080" alt="hasil 3" src="https://github.com/user-attachments/assets/5d81b98a-145d-4183-9759-7a78af6242c4" />



### Langkah 4: Membuat CSS Eksternal 
Membuat file CSS terpisah untuk mengatur tata letak navigasi, warna latar belakang, serta efek hover pada menu. File eksternal dihubungkan menggunakan tag `<link>`.

<img width="1920" height="1080" alt="code 4" src="https://github.com/user-attachments/assets/04c3b586-2b3d-49ba-98e2-5d31bb47c93f" />
<img width="1920" height="1080" alt="code 4 lnjutan" src="https://github.com/user-attachments/assets/76de10e4-c6e2-442a-bf04-86971c9ab250" />
<img width="1920" height="1080" alt="hasil 4" src="https://github.com/user-attachments/assets/b0816a15-b837-4d75-bbab-4b53be758ba6" />


### Langkah 5: Menambahkan CSS Selector (ID dan Class Selector)
Menggunakan ID Selector (`#intro`, `#intro h1`) dan Class Selector (`.button`) pada file `style_eksternal.css` untuk memberikan gaya spesifik pada elemen kontainer utama dan tombol tautan.

<img width="1920" height="1080" alt="code 5" src="https://github.com/user-attachments/assets/9fd06af9-4aca-4442-9ad7-6a66eaaff7a8" />
<img width="1920" height="1080" alt="hasil 5" src="https://github.com/user-attachments/assets/f26d2627-9167-469c-a438-c2f72553295b" />

## Langkah 6: Validasi file css
Memvalidasi melalui website : https://jigsaw.w3.org/css-validator/ 
   <img width="1920" height="1080" alt="validasi" src="https://github.com/user-attachments/assets/d2dae576-5a07-4752-beaa-30a479f946f9" />


## 3. Pertanyaan dan Tugas

1. **Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS.**
   *Experiment memindahkan letak text **Hello World** menjadi berada di tengah halaman, menambahkan efek hover pada tag `a` yang memiliki class `.button`
     <img width="798" height="124" alt="tugas1" src="https://github.com/user-attachments/assets/bf8717c7-66a0-4c12-9850-b67fd0665fbe" />
     <img width="843" height="708" alt="jawaban1" src="https://github.com/user-attachments/assets/4afc3e30-4f91-4987-87fe-254a02c0c685" />


2. **Apa perbedaan pendeklarasian CSS elemen `h1 {...}` dengan `#intro h1 {...}`? Berikan penjelasannya!**
   * *Jawaban:* 
     * `h1 {...}` adalah **Element Selector** yang akanmenerapkan aturan gaya ke **seluruh** tag `h1` di dalam dokumen HTML.
     * `#intro h1 {...}` adalah **Descendant / Combined Selector** yang hanya akan menerapkan aturan gaya pada tag `h1` yang berada **di dalam** elemen yang memiliki ID `intro`. Selector ini memiliki tingkat spesifisitas yang lebih tinggi dibandingkan element selector biasa.

3. **Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!**
   * *Jawaban:* Yang akan ditampilkan dan diprioritaskan adalah **Inline CSS**, kemudian **Internal/Eksternal CSS**. Aturan umum dalam CSS menempatkan *Inline Style* pada prioritas tertinggi karena ditulis langsung pada elemen tersebut. Contoh : 

     <img width="531" height="129" alt="tugas2-1" src="https://github.com/user-attachments/assets/64a313ef-1ee3-44f1-8ae7-875b00bd07c6" />
      <img width="714" height="78" alt="tugas2" src="https://github.com/user-attachments/assets/b3c989ad-0c6b-40c1-b821-9645b31e407a" />
      <img width="830" height="891" alt="jawaban2" src="https://github.com/user-attachments/assets/7bdf1034-3796-4165-a1e1-5d4030f55921" />

4. **Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! (`<p id="deklarasi-id" class="deklarasi-class">`)**
   * *Jawaban:* Deklarasi dari **ID Selector** akan lebih diprioritaskan dibandingkan **Class Selector**. Hal ini dikarenakan ID memiliki tingkat spesifisitas (specificity weight) yang jauh lebih tinggi daripada Class dalam hierarki CSS. Contoh :
   <img width="367" height="200" alt="tugas3-1" src="https://github.com/user-attachments/assets/0a3d9a3f-1d7e-48a2-8fd0-40e78c24ce48" />
  <img width="1095" height="186" alt="tugas3" src="https://github.com/user-attachments/assets/bc340224-9a14-49c9-9cd5-520b9ae79af1" />
  <img width="824" height="829" alt="jawaban3" src="https://github.com/user-attachments/assets/a4694aa2-6cdb-4811-8554-a2a67b7e46a8" />

# Praktikum 4: CSS Layout (Box Element & Layout Sederhana) - Pemrograman Web
Repository ini dibuat untuk menyelesaikan tugas Praktikum 4 Pemrograman Web.

## Identitas Mahasiswa

| Keterangan      | Data                 |
| --------------- | -------------------- |
| **Nama**        | Najhan Said Ziddan |
| **Kelas**       | I251D                |
| **NIM**         | 312510367            |
| **Mata Kuliah** | Pemrograman Web      |
| **Dosen**       | Agung Nugroho, S.Kom., M.Kom. |

### Tujuan Praktikum

Mahasiswa mampu memahami konsep box element pada CSS (float dan clearfix).

Mahasiswa mampu membuat layout website sederhana menggunakan semantic element HTML5.

Mahasiswa mampu mengatur navigasi, hero panel, main content, sidebar, dan footer menggunakan CSS.

Mahasiswa mampu membuat halaman tambahan (About dan Kontak) dengan layout yang konsisten.

---

## Struktur Folder Proyek

```
Lab4Web/
├── Lab4_Layout/
│   ├── Lab4_Layout.html
│   ├── about.html
│   ├── kontak.html
│   └── style.css
├── Lab4web/
│   └── Lab4_box.html
└── README.md
```

<img width="344" height="281" alt="ss file leb4" src="https://github.com/user-attachments/assets/d30312b6-b3da-40fa-bc20-ff035e5ee3f5" />


---

## Langkah-langkah Praktikum

### 1. Membuat Box Element (`Lab4_box.html`)

Langkah pertama adalah menyiapkan dokumen HTML dasar dengan nama `Lab4_box.html` yang berisi `<header>` dengan judul "Box Element".
<img width="1046" height="385" alt="ss1" src="https://github.com/user-attachments/assets/303f1f3a-43ff-4c4e-8113-689f7a71ee5f" />


Kemudian di dalam `<body>` ditambahkan `<section>` yang berisi empat buah `<div>` dengan class `div1` sampai `div4`.

<img width="439" height="162" alt="ss2" src="https://github.com/user-attachments/assets/e29ae351-a44f-48d3-88e6-4a09847c06c2" />


#### CSS Float Property

Pada bagian `<head>` ditambahkan CSS internal untuk membuat float element:

- Semua `div` diberi `float: left` dan `padding: 10px`.
- `.div1` berwarna merah, `.div2` kuning, `.div3` hijau.
- `.div4` berwarna biru dengan `clear: left` dan `float: none` (clearfix) agar tampil di baris baru.

<img width="781" height="468" alt="ss3" src="https://github.com/user-attachments/assets/ae27b99f-1d00-4c58-a44c-527fe02bbd77" />


Hasil di browser: Div1, Div2, dan Div3 tampil sejajar ke samping, sedangkan Div4 berada di bawahnya dengan lebar penuh.

<img width="1019" height="337" alt="ss4" src="https://github.com/user-attachments/assets/940f9539-2ed6-4ad1-80b8-cd05ac0dafb0" />


---

### 2. Membuat Layout Sederhana (`Lab4_Layout.html`)

Membuat kerangka layout menggunakan semantic element. Dokumen ini menghubungkan file `style.css` dan memiliki `<div id="container">` sebagai pembungkus utama.

<img width="785" height="199" alt="ss5" src="https://github.com/user-attachments/assets/9f2b7df4-bb71-49da-93ec-7995406d5ce1" />


Di dalam container ditambahkan elemen `<header>`, `<nav>` (Home, Artikel, About, Kontak), `<section id="hero">`, `<section id="wrapper">` (berisi `<section id="main">` dan `<aside id="sidebar">`), serta `<footer>`.

<img width="373" height="123" alt="ss6" src="https://github.com/user-attachments/assets/71a6d9f9-74ce-4d12-b411-be868ec439b3" />

<img width="631" height="410" alt="ss7" src="https://github.com/user-attachments/assets/0e2b2592-5f63-417f-8de7-f3f3ddfd4d6d" />



Hasil sebelum diberi CSS:

<img width="943" height="486" alt="ss8" src="https://github.com/user-attachments/assets/a24cc0b2-0e97-4270-af8d-86c7dc4bf8e0" />


---

### 3. Menambahkan CSS Layout (`style.css`)

CSS ditambahkan untuk membuat tampilan dasar layout, meliputi:

- `@import` Google Font **Open Sans** dan **Open Sans Condensed**.
- Reset CSS (`margin: 0; padding: 0`).
- Pengaturan `body` (font-size, font-family, warna teks).
- `#container` dengan lebar `980px`, rata tengah (`margin: 0 auto`), dan `box-shadow`.
- Pengaturan `header` dan `header h1`.

<img width="907" height="556" alt="ss9" src="https://github.com/user-attachments/assets/b0155273-1ff2-4241-85b2-35ca756f52fe" />

Hasil di browser:

<img width="1346" height="394" alt="ss10" src="https://github.com/user-attachments/assets/1c726f0b-5179-4f1c-a571-6b6c3a339144" />

---

### 4. Mengatur Navigasi

CSS navigasi dibuat dengan ketentuan:

- `nav` memiliki background biru (`#1f5faa`).
- Link `nav a` ditampilkan `inline-block`, berwarna putih, tebal, tanpa garis bawah.
- `nav a.active` dan `nav a:hover` memiliki background `#2b83ea`.

<img width="478" height="402" alt="ss11" src="https://github.com/user-attachments/assets/2503fe89-04a1-48c5-a657-2ed90835f667" />

<img width="1365" height="423" alt="ss12" src="https://github.com/user-attachments/assets/b84019f6-fd1e-4c6f-b484-6de138717df3" />


---

### 5. Membuat Hero Panel

Menambahkan kode HTML pada `<section id="hero">` berisi judul, paragraf, dan tombol "Learn more", lalu diberi style: background abu-abu (`#e4e4e5`), padding, serta pengaturan ukuran font `h1` dan `p`.

<img width="787" height="226" alt="ss13" src="https://github.com/user-attachments/assets/def175a2-9a95-40e4-a8ba-691ac519c15e" />

<img width="361" height="351" alt="ss14" src="https://github.com/user-attachments/assets/123694dd-9e59-464a-9775-fefac1d1219a" />

<img width="1363" height="658" alt="ss15" src="https://github.com/user-attachments/assets/04b3dc38-38ec-4ca7-bd03-0e419878a019" />



---

### 6. Menambahkan CSS Float untuk Main Content dan Sidebar

- `#main` dan `#sidebar` menggunakan `float: left`.
- Lebar `#main` = `640px`, lebar `#sidebar` = `260px`, keduanya dengan `padding: 20px`.
- Sidebar berisi dua `widget-box` (daftar link dan teks) yang diberi style border, title berwarna biru (`#428bca`), list tanpa bullet, dan efek hover.

<img width="705" height="288" alt="pijet" src="https://github.com/user-attachments/assets/07b3c9a3-78ae-450a-8bd9-e6f4e5642060" />

<img width="337" height="576" alt="ss18" src="https://github.com/user-attachments/assets/bacd60af-5db5-4e36-922b-ff8cd373fa2e" />


<img width="361" height="413" alt="image" src="https://github.com/user-attachments/assets/86ef685a-47ed-43b1-b265-9b225c4bf1d4" />


---

### 7. Mengubah Tampilan Footer

Footer diberi style background gelap dengan teks putih agar terlihat berbeda dari konten utama.

<img width="442" height="63" alt="ss20" src="https://github.com/user-attachments/assets/b4bacaf1-4dbb-41ed-b3ee-fc84935fb6a2" />

<img width="291" height="136" alt="image" src="https://github.com/user-attachments/assets/49d054de-5563-42d0-9ff9-3fd67e06e31d" />

---

### 8. Menambahkan Elemen Lain pada Main Content

Menambahkan `div.row` yang berisi tiga `div.box`. Masing-masing box memiliki gambar, heading, paragraf, dan tombol "View detail". CSS yang digunakan:

- `.box` dengan `float: left`, `width: 33.333333%`, `box-sizing: border-box`, dan `text-align: center`.
- `.image-circle` dengan `border-radius: 50%` agar gambar berbentuk lingkaran.
- `.row` dengan margin negatif dan clearfix (`:before` dan `:after` dengan `display: table` dan `clear: both`).

<img width="875" height="567" alt="ss21" src="https://github.com/user-attachments/assets/d9ab6c79-dcd5-4743-beef-4cb39e38fc9f" />


<img width="319" height="375" alt="ss23" src="https://github.com/user-attachments/assets/e65ebd3a-9220-42d2-9b5e-1a2880686b60" />

<img width="363" height="583" alt="ss22" src="https://github.com/user-attachments/assets/ad1794d1-255f-441f-b59e-7ade7255781d" />


<img width="322" height="272" alt="image" src="https://github.com/user-attachments/assets/26d56f2f-edb4-4cf1-b944-71b15aea41a8" />


---

### 9. Membuat Content Artikel

Menambahkan dua `<article class="entry">` yang dipisah dengan `<hr class="divider">`. Artikel pertama memiliki gambar di kiri, sedangkan artikel kedua memakai class `right-img` sehingga gambar berada di kanan.

CSS `.entry`:
- `margin: 15px 0`, `h2` dengan `margin-bottom: 20px`, dan `p` dengan `line-height: 25px`.
- `.entry img` menggunakan `float: left`, `border-radius: 5px`, dan `margin-right: 15px`.
- `.entry .right-img` menggunakan `float: right` dengan margin kiri `15px`.

<img width="612" height="540" alt="ss25" src="https://github.com/user-attachments/assets/20132ffd-e6ec-4629-b59a-021c55c69143" />

<img width="399" height="379" alt="ss26" src="https://github.com/user-attachments/assets/296f2580-292b-4384-bf9b-1c5dfbfccc5e" />

<img width="1361" height="718" alt="ss27" src="https://github.com/user-attachments/assets/668d0f02-3a9e-4a20-8384-0f5abe1dbb50" />


---

## Pertanyaan dan Tugas

### 1. Menambahkan Menu About (`about.html`)

Membuat halaman About dengan layout yang sama (header, nav, hero, main, footer). Halaman ini berisi bagian **Tentang Saya** (hero), **Deskripsi Diri**, dan **Portfolio** (Website Layout Sederhana, Desain UI/UX, dan Project Pemrograman). Menu "About" diberi `class="active"`.

<img width="479" height="560" alt="image" src="https://github.com/user-attachments/assets/8bfb6db2-3b5f-467e-a6f5-b8374ce564b9" />


<img width="386" height="457" alt="image" src="https://github.com/user-attachments/assets/c235551c-be26-44cf-bbfe-70aed802ca9f" />


<img width="1365" height="715" alt="ss29" src="https://github.com/user-attachments/assets/88fe8ec0-b80a-4516-92b2-f83675c54904" />



### 2. Menambahkan Menu Kontak (`kontak.html`)

Membuat halaman Kontak yang berisi **Form Contact** dengan field Nama Lengkap, Email, Subjek, dan Pesan (textarea), serta tombol "Kirim Pesan". Semua field menggunakan atribut `required`, dan menu "Kontak" diberi `class="active"`.

<img width="416" height="671" alt="ss30" src="https://github.com/user-attachments/assets/2b6fef34-726d-453e-b218-55cc2f3cb81d" />



<img width="1260" height="718" alt="ss31" src="https://github.com/user-attachments/assets/d7a9c2de-1944-40bd-820e-aa078c4a7266" />



---

## Kesimpulan

Pada praktikum ini telah dipelajari cara membuat layout website dengan CSS menggunakan properti `float` dan `clear`, penggunaan semantic element HTML5, serta pembuatan komponen seperti navigasi, hero panel, sidebar widget, box, dan artikel. Selain itu juga dibuat halaman About dan Kontak dengan layout yang konsisten.

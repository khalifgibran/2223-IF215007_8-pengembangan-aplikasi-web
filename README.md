# Resume Canvas HTML 5
# Pengenalan
 Canvas adalah elemen yang termasuk ke bagian dari HTML5. Di canvas juga kita dapat merender 2D dan gambar dari bitmap dan memungkinkan untuk dinamis, skrip render bentuk 2D dan gambar bitmap.

1. Cara menggambar di canvas

 Objek ctx jika di seni rupa dapat dirupakan sebagai pensil. Objek ini memiliki beberapa method untuk menggambar di canvas seperti fillRect(), arc(), fillText(), dsb.
  Untuk menggambar dengan method-method tersebut kita harus menentukan dulu koordinat titik x dan y nya. Karena canvas terdiri dari kumpulan piksel yang membentuk diagram kartesius terbalik.

2. Menggambar titik pada canvas

 Dalam seni rupa, titik adalah bagian terkecil dari sebuah objek yang menempati suatu ruang. Sedangkan dalam komputer titik adalah ukuran 1 piksel dari layar.
Untuk menggambar titik pada canvas, kita dapat menggunakan method fillRect() dengan ukuran 1x1 piksel.

ctx.fillRect(x,y,1,1);

Variabel x dan y kita ganti dengan nilai koordinatnya, misalkan kita ingin menggambar titik pada koordinat (10,10).

3. Menggambar persegi pada canvas

Ada tiga fungsi yang digunakan untuk menggambar persegi pada canvas:

- ctx.strokeRect(x,y,w,h) persegi dengan garis (outline) saja.
- ctx.fillRect(x,y,w,h) persegi dengan polesan warna (default-nya hitam).
- ctx.clearRect(x,y,w,h) persegi transparan untuk menghapus.

Seperti biasa, kita harus memberikan titik koordinat x dan y. Sementara nilai w dan h untuk lebar dan tingginya.

4. Menyisipkan teks pada canvas

Ada dua fungsi untuk membuat teks:

1. strokeText() untuk teks dengan garis luar (outline) saja.
2. illText() untuk teks dengan warna (default hitam).

Fungsi tersebut memiliki tiga parameter yang wajib diberikan:

ctx.fillText("Teks yang akan dibuat", x, y);

5. Merender gambar pada canvas
Untuk melakukannya, kita membutuhkan sebuah gambar dan menggunakan fungsi drawImage() untuk merender-nya ke canvas.

drawImage(img, x, y);

Kita akan menggunakan gambar dari : Al-Amin Basketball logo.png

Pertama buat elemen <img>:

<p>Gambar yang akan di-render:</p>
<img id="scream" src=""D:\My Project 1.0\Al-Amin Basketball logo.png"" alt="The Scream" width="220" height="277">
- Kemudian buat tombol render:

<p><button onclick="renderImage()">Render Image</button></p>
Terakhir membuat fungsi renderImage():

function renderImage() {
    var canvas = document.getElementById("myCanvas");
    var ctx = canvas.getContext("2d");

    // ambil gambar dari elemen <img>
    var img = document.getElementById("scream");

    // render ke Canvas
    ctx.drawImage(img,10,10);
}

# Pemrograman Game Berbasis HTML5
Untuk membuat game berbasis HTML5 dari nol, karena hanya pengenalan saja.

- Membuat objek secara acak di Canvas
- Cara Membuat Animasi di Canvas;
- Cara Membuat Gravitasi dan Menerapkan Elemen Fisika Lainnya;
- Cara Memutar Audio untuk Game;
- ogika Game dan sistem Poin;
- Logika Kode untuk Benturan (Collision);
Bila kamu tidak ingin membuat semua itu dari nol, gunakanlah Game Engine. Karena sudah dibuatkan di sana dan kita tinggal pakai saja.

# Pemrograman Grafis atau Grafika Komputer
untuk pemrograman grafis, bisa dicoba berikut:

- Membuat Aplikasi Painting Berbasis HTML5;
- Membuat Photoshop sendiri;
- Menerapkan algoritma grafika komputer seperti algoritma membuat garis;
- Pengolahan Citra dan Computer Vision;
- Membuat Diagram Interaktif;
- Me-render Gambar dari Webcam ke Canvas

# Praktikum Web 5
## Langkah-langkah Praktikum
### Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mengenal javascript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World");
</script>
</body>
</html>
```

- Output :
![prak5_html1](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/6d9d4b49-5eea-483b-8895-2efae82872f1)

### Javascrip Dasar
- Pemakaian Alert sebagai property window.

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>alert box</title>
</head>
<body>
    <script language="javascript">
        window.alert("Ini sebuah pesan untuk anda")
    </script>
</body>
</html>
```

- Output:
![prak5_html2](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/daf6450a-08e7-4db3-a1ca-795a25b55a36)

### Pemakaian method dalam objek
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>script javascript</title>
</head>
<body>
    Percobaan Memakai javascript : <br>
    <script language="javascript">
        document.write("Selamat Mencoba Javascript <br>");
        document.write("Semoga Sukses");
    </script>
</body>
</html>
```

- Output:
![prak5_html3](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/9cd24c3d-dd48-4194-bb43-d0d1e813173f)

### Pemakaian Prompt

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>pemasukan data</title>
</head>
<body>
    <script language="javascript">
        var nama = prompt("Siapa nama anda?", "Masukan nama anda");
        document.write("hai, " + nama )
    </script>
</body>
</html>
```

- Output :
![prak5_html4](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/eacdb2fe-6913-4f95-ae74-81688417156b)

### Pembuatan fungsi dan cara pemanggilannya
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program javascript</title>
    <script language = "javascript">
        function pesan() {
            alert ("Memanggil javascript lewat body onload")
        }
    </script>
</head>
<body onload= pesan()>
</body>
</html>
```

- Output :
![prak5_html5](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/b93fad1a-2433-4b1e-b632-6729b2c44e82)

### Dasar Pemrograman Di Javascript
- Operasi dasar aritmatika
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program javascript</title>
</head>
<body>
    <input type="button" name="button1" value="hitung" onclick=test(27,5)>
</body>
<script language="javascript">
        function test (val1, val2)
        {
            document.write("<br>" + "perkalian = val1*val2" + "<br>")
            document.write(val1*val2)
            document.write("<br>" + "pembagian = val1:val2" + "<br>")
            document.write(val1/val2)
            document.write("<br>" + "penjumlahan = val1*val2" + "<br>")
            document.write(val1+val2)
            document.write("<br>" + "pengurangan = val1-val2" + "<br>")
            document.write(val1-val2)
            document.write("<br>" + "modulus = val1%val2" + "<br>")
            document.write(val1%val2)
        }
</script>
</html>
```
- Output :
![prak5_html6](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/4c1d37f2-174b-4325-a719-66e3663bb010)

### Seleksi kondisi (if..else)
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Belajar JS</title>
</head>
<body>
    <h1>BELAJAR JS</h1>
</body>
<script>
    var nilai = prompt("masukan nilai (0-100): ");
    var hasil = " ";
    if (nilai >= 75)
        hasil = "lulus";
    else
        hasil="gagal";
document.write("KKM 75<br>");
document.write("hasil : ",nilai," ", hasil);
</script>
</html>
```

- Output :

![prak5_html7](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/21d2b461-794c-449d-a63c-d11e3839579c)

![prak5_html8](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/3cfa116c-926f-4beb-8530-6a0842683e0c)

### Penggunaan operator switch untuk seleksi kondisi
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh program javascript</title>
    <script language="javascript">
        function test()
        {
            val1 = window.prompt("Input nilai (1-9): ")
            switch (val1)
            {
                case "1":
                    document.write("bilangin Satu")
                    break
                case "2":
                    document.write("bilangin Dua")
                    break
                case "3":
                    document.write("bilangin Tiga")
                    break
                case "4":
                    document.write("bilangin Empat")
                    break
                case "5":
                    document.write("bilangin Lima")
                    break
                default:
                    document.write("bilangan lainnya")
                
            }
        }
    </script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```

_ Output :

- 1. Jika di isi

![prak5_html9 1](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/3b4a4974-303e-4936-accb-a50e4143617e)

![prak5_html9 2](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/828b12d5-b02a-4fbf-b835-71ef095e0fba)

- 2. Jika tidak di isi

![prak5_html9 3](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/2b617c48-2770-4a97-8953-52b720bf00f0)

![prak5_html9 4](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/4d9e9f46-55fb-4532-ad13-ae0df49e70cb)

### Pembuatan Form
- Form Input
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script language="javascript">
        function test () {
            var val1 = document.kirim.T1.value
            if (val1%2 == 0)
            document.kirim.T2.value="Bilangan genap"
            else
            document.kirim.T2.value="Bilangan ganjil"
        }
    </script>
</head>
<body>
    <from method="post" name="kirim">
        <p> BIL <input type="text" name="T1" size="20"> 
        Merupakan BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </from>
</body>
</html>
```

- output :

![prak5_html10 1](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/a7293084-03d0-4ec6-8015-cfa890f9f899)

![prak5_html10 2](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/87c44ec3-f319-43a0-aa1e-d6147996a58b)

### Form Button.
```
<!DOCTYPE html>
<html lang="en">
<head> 
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Object Document</title>
</head>
<body>
    <script language="javascript">
    function ubahwarnaLB(warna) {
        document.bgColor = warna;
    }
    function ubahwarnaLD(warna) {
        document.fgColor = warna;
    }
    </script>
    <h1>TES</h1>
    <from>
        <input type="button" value="Latar belakang hijau" onclick="ubahwarnaLB('green')">
        <input type="button" value="Latar belakang putih" onclick="ubahwarnaLB('white')">
        <input type="button" value="Text Kuning" onclick="ubahwarnaLD('yellow')">
        <input type="button" value="Text Biru" onclick="ubahwarnaLD('blue')">
    </from>
    <script language="javascript">
        document.write("dimodifikasi terakhir pada" + document.lastModified);
    </script>
</body>
</html>
```

- Output :

- Klik latar belakang hijau

![prak5_html11 1](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/052cc088-5ae1-4c4f-ae26-0da6d93d49f6)

- Klik latar belakang putih

![prak5_html11 2](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/3f06dbad-a465-4a52-ad03-411bdf7bbfa1)

- klik Text Kuning

![prak5_html11 3](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/c92d46d0-137c-4e92-a956-427443132606)

- Klik Text Biru

![prak5_html11 4](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/f7738b48-c2ec-4dd8-866f-8a299265029b)

### HTML DOM
- Pilihan menggunakan checkBox dengan perhitungan otomatis
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daftar Menu</title>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="Menu1" onclick="hitung(this) ;"/>Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="Menu2" onclick="hitung(this) ;" />Tempe Goreng Rp. 500</label><br />
    <label><input type="checkbox" value="2500" id="Menu3" onclick="hitung(this) ;" />Telur Dadar Rp. 2.500</label><hr />
    <strong>Total Bayar : Rp.<input id="total" type="text" /></strong>
</body>
<script>
    function hitung(ele) {
        var total = document.getElementById("total").value;
            total = (total ? parseInt(total):0);
        var harga = 0;

        if (ele.checked) {
            harga = ele.value;
            total += parseInt(harga);
        } 
        else {
            harga = ele.value;
            if(total > 0)
                total -= parseInt(harga);
        }
        document.getElementById("total").value = total;
    }
</script>
</html>
```
- Output :
![prak5_html12](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/e86fc8d6-ba94-42bd-882d-6ab091fbbdae)

### Pertanyaan dan Tugas
### Buat script untuk melakukan validasi pada isian form.
![prak5_html13](https://github.com/mullf/Lab5_Js_HTML_ProgWeb/assets/115521049/e3b2dac7-0bea-4aee-b85c-b809a651ec67)

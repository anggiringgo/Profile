**PRAKTIKUM 5**

**Membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut**
```
<!DOCTYPE html>
<html lang="en">
<head>
<title>Mengenal JavaScript</title>
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
![Screenshot (112)](https://user-images.githubusercontent.com/81580084/116057417-fa5c4680-a6a8-11eb-840c-c1313dc3f1bc.png)

**Pemakaian Alert sebagai property window**
```
<html>
<head>
<title>alert box>/title>
</head>
<script language="javascript">
<!--
window.alert("ini merupakan pesan untuk anda");
//-->
</script>
</body>
</html>
```
![Screenshot (113)](https://user-images.githubusercontent.com/81580084/116058102-b0279500-a6a9-11eb-8fb4-f6dcfd0fb527.png)

**Pemakaian method dalam objek**
```
<html>
<head>
<title>skrip javascript>/title>
</head>
<body>
percobaan memakai javascript: <br>
<script language="javascript">
<!--
document.write("selamat mencoba javascript<br>");
document.write("seoga sukses");
//-->
</script>
</body>
</html>
```
![Screenshot (114)](https://user-images.githubusercontent.com/81580084/116058775-5e333f00-a6aa-11eb-807c-473cf19e7112.png)

**Pemakaian Prompt**
```
<html>
<head>
<title>contoh pemasukan data>/title>
</head>
<body>
<script lang="javascript">
var nama=prompt("siapa nama anda?","masukan nama anda");
document.write("hai, "+ nama);
</script>
</body>
</html>
```
![Screenshot (117)](https://user-images.githubusercontent.com/81580084/116059338-ee718400-a6aa-11eb-9591-1183e8c91422.png)
![Screenshot (116)](https://user-images.githubusercontent.com/81580084/116059431-06490800-a6ab-11eb-9d49-6971b03ce6fa.png)

**Pembuatan fungsi dan cara pemanggilannya**
```
<html>
<head>
<title>contoh program javascript</title>
<script lang="javascript">
funtion pesan(){
alert("memanggil javascript lewat body onload")
}
</script>
</head>
<body onload=pesan()>
</body>
</html>
```
![Screenshot (131)](https://user-images.githubusercontent.com/81580084/116061581-3b565a00-a6ad-11eb-9eaa-1ba48f7c26df.png)

**Operasi dasar aritmatika**
```
<html>
<head>
<title>contoh program javascript</title>
<script lang="javascript">
function test (val1,val2)
{
document.write("<br>"+"perkalian : val1*val2 "+"<br>")
document.write(val1*val2)
document.write("<br>"+"perkalian : val1/val2 "+"<br>")
document.write(val1/val2)
document.write("<br>"+"perkalian : val1+val2 "+"<br>")
document.write(val1+val2)
document.write("<br>"+"perkalian : val1-val2 "+"<br>")
document.write(val1-val2)
document.write("<br>"+"perkalian : val1%val2 "+"<br>")
document.write(val1%val2)
}
</script>
</head>
<input type="buttob" name="nutton1 value+"aritmetchic" onclick=test(9,4)>
</body>
</html>
```
![Screenshot (134)](https://user-images.githubusercontent.com/81580084/116063375-195dd700-a6af-11eb-84a8-5a58acd3c561.png)
![Screenshot (135)](https://user-images.githubusercontent.com/81580084/116063387-1b279a80-a6af-11eb-9b7a-ed7be28d6dde.png)

**Seleksi kondisi (if..else)**
```
<html>
<head>
<title>contoh if else</title>
</head>
<body>
<script lang="javascript">
var nilai = prompt ("nilai (0-100): ", 0);
var hasil = "";
if (nilai>=60)
hasil = "lulus";
else
hasil = "tidak lulus";
document.write("hasil: "+ hasil);
</script>
</body>
</html>
```
![Screenshot (118)](https://user-images.githubusercontent.com/81580084/116064219-fed82d80-a6af-11eb-9d29-e176d1df1969.png)
![Screenshot (119)](https://user-images.githubusercontent.com/81580084/116064232-01d31e00-a6b0-11eb-8528-684a42c3cbd2.png)

**Penggunaan operator switch untuk seleksi kondisi**
```
<html>
<head>
<title>contoh program javascript</title>
<script language="JavaScript">
    function test ()
    {
        val1=window.prompt("input nilai (1-5):")
        switch (val1)
        {
            case "1" :
                document.write("bilangan satu")
                break
            case "2" :
                document.write("bilangan dua")
                break
            case "3" :
                document.write("bilangan tiga")
                break
            case "4" :
                document.write("bilangan empat")
                break
            case "5" :
                document.write("bilangan lima")
                break
            default :
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
 ![Screenshot (124)](https://user-images.githubusercontent.com/81580084/116066195-fb45a600-a6b1-11eb-8a45-623c2be23ec6.png)
   
   
   **Pembuatan Form**
```
 <!DOCTYPE html>
<html lang="en">
<head>
	<title>Daftar Menu</title>
<script language="JavaScript">
 	function test () {
 		var val1=document.kirim.T1.value
 		if (val1%2==0)
 			document.kirim.T2.value="bilangan genap"
 		else
 			document.kirim.T2.value="bilangan ganjil"
 	}
 </script>
  <script>
 	function hitung(ele) {
 		var total = document.getElementById('total').value;
 			total = (total ? parseInt(total) : 0);
 		var harga = 0;

 		if (ele.checked) {
 			harga = ele.value;
 			if (total > 0)
 				total -= parseInt(harga);
 		}
 		document.getElementById('total').value = total;
 	}
 </script>
</head>
<body>
<form method="POST" name="kirim">
		<p>BIL <input type="text" name="T1" size="20"> MERUPAKAN BIL <input type="text" name="T2" size="20"required minlength="Mohon Isi"></p>
		<p><input type="button" value="TEBAK" name="B1" onclick=test()></p>	
</form>
<script language="JavaScript">
 	<!--
 		function ubahWarnaLB(warna) {
 			document.bgColor = warna;
 		}
 		function ubahWarnaLD(warna) {
 			document.fgColor = warna;
 		}
 	//-->
 </script>
 <h1>tes</h1>
<form>
	<input type="button" value="Latar Belakang Biru" onclick="ubahWarnaLB('BLUE')">
	<input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
	<input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
	<input type="button" value="Teks Putih" onclick="ubahWarnaLD('WHITE')">
</form>
<script language="JavaScript">
	<!--
		document.write("Dimodifikasi terakhir pada " + document.lastModified);
		//-->
</script>
<h1>Daftar Menu Makanan</h1>
 <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this) ;" />Ayam Goreng Rp. 15.000</label><br />
 <label><input type="checkbox" value="5000" id="menu2" onclick="hitung(this) ;" />Tempe Goreng Rp. 2.000</label><br />
 <label><input type="checkbox" value="5000" id="menu3" onclick="hitung(this) ;" />Telur Dadar Rp. 10.000</label><br />
 <strong>Total Bayar: Rp. <input id="Total" type="Text"></strong>
</body>
</html> 
```
![Screenshot (127)](https://user-images.githubusercontent.com/81580084/116066495-55df0200-a6b2-11eb-8945-af67d9f40163.png)

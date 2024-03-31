```sh
Syarat tugas :
- Membuat repostiory di GitHub dengan nama "devops20-dumbways-<nama>"
- Membuat folder task per harinya dengan file "README.md" (bisa dibuat per folder/directory)

Task :
1. Buat 3 directory yang masing-masing berisi 2 file dan rapihkan sebaik mungkin!
2. Penjelasan text manipulation beserta step by step
3. Penjelasan tool htop atau nmon
4. buatlah BASH Script untuk instalasi nginx

```
Answer
# **1.**

# **2.**
## **Teks Manipulation**
merupakan suatu method untuk memanipulasi sebuah file menggunakan terminal tanpa menggunakan teks editor seperti **nano**. Berikut Contoh **Perintah Teks Manipulation**
**1. cat**
Cat adalah salah satu perintah yang berfungsi untuk membuat daftar konten atau isi file pada standard output (sdout). Yang kalian tahu pasti perintah cat hanya bisa untuk melihat isi dari suatu file, sebenarnya tidak hanya itu.

Contoh penggunaan :

```sh
cat (file-name)
```

<p aligh="center">
<img src="../Week 2/image task2/Cat file.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk melihat isi dari suatu file

```sh
cat > (file-name)
```

<p aligh="center">
<img src="../Week 2/image task2/cat - file.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk membuat suatu file baru serta memasukkan teks, Jika sudah menambakan teks kalian dapat keluar dengan klik CTRL + C.

```sh
cat file1 file2 > file3
```

<p aligh="center">
<img src="../Week 2/image task2/cat gabung file.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk menggabungkan dua buah file, dan menyimpannya ke dalam file3

**2. sed​**
Sed adalah singkatan dari stream editor. Gunanya untuk memanipulasi teks dasar pada file. Dengan sed kita dapat mengganti teks dengan cepat.

Contoh penggunaan :

```sh
sed -i 's/Hello/Holla/g' file3
```

<p aligh="center">
<img src="../Week 2/image task2/sed.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : mengganti semua kata Hello menjadi Holla pada file3

**3. grep​**
Grep merupakan perintah untuk melakukan pencarian sebuah text dalam sebuah file yang telah dibuat.

Contoh penggunaan :

```sh
grep Dumbways file3
```

<p aligh="center">
<img src="../Week 2/image task2/grep.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : akan mencari kata Dumbways pada file3

```sh
grep -c Dumbways file3
```

<p aligh="center">
<img src="../Week 2/image task2/grep count.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : akan menghitung jumlah kata “Dumbways” pada filetiga

```sh
grep Dumbways *
```

<p aligh="center">
<img src="../Week 2/image task2/grep count all direc.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : akan mencari semua file yang berisikan kata Dumbways

**4. sort​**
Sort untuk mengurutkan data, baik itu secara ascending atau descending.

Berikut adalah contoh penggunaan :

```sh
sort file4
```
<p aligh="center">
<img src="../Week 2/image task2/sort ascending.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk mengurutkan berdasarkan ascending

```sh
sort -r file4
```

<p aligh="center">
<img src="../Week 2/image task2/sort descending.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk mengurutkan berdasarkan descending

**5. echo​**
Echo digunakan untuk mencetak string / pesan dari hasil perintah lain.

Berikut adalah contoh penggunaan

```sh
echo "Hello Dumbways!"
```

<p aligh="center">
<img src="../Week 2/image task2/echo text.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk mencetak string **

```sh
echo "Hello Dumbways!" >> file3
```

<p aligh="center">
<img src="../Week 2/image task2/addtext with echo.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk mencetak kata Hello Dumbways! di file3

```sh
echo "Replace semua data" > file5
```

<p aligh="center">
<img src="../Week 2/image task2/echo replace text.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

keterangan : untuk mereplace semua data di file5 dan menggantinya dengan "Replace semua data"
# **3.**
**htop**

merupakan perintah untuk memonitoring sistem (memory, cpu, swap)

```sh
htop
```

<p aligh="center">
<img src="../Week 2/image task2/htop monitoring.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

lakukan installasi dengan command berikut
```sh
sudo apt install htop -y
```
<p aligh="center">
<img src="../Week 2/image task2/htop.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

Keterangan : 
- CPU adalah berapa jumlah core yang kita miliki.
- Mem adalah total penggunaan memory.
- Swp adalah Memory cadangan.
- Tasks adalah aplikasi yang sedang berjalan di server.
- Load average adalah rata-rata aplikasi yang berjalan.
- Uptime adalah berapa lama server kita hidup.
- PID adalah nomor proses id setiap proses yang berjalan di linux.
- VIRT adalah memory yang terpakai.
- Command adalah perintah apa yang sedang di jalankan.

**nmon**
merupakan perintah untuk memonitoring sistem (memory, cpu, swap)
```sh
nmon
```

install menggunakan command :

```sh
sudo apt install nmon -y
```
<p aligh="center">
<img src="../Week 2/image task2/install nmon.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>


Kita dapat memilih ingin memonitoring apa saja, Disini kita coba saja untuk menampilkan beberapa saja.

c adalah CPU
m adalah Memory
d adalah Disk
n adalah network
Berikut adalah tampilan dari nmon untuk menampilkan cpu, memory, disk, dan network

<p aligh="center">
<img src="../Week 2/image task2/nmon.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

# **4.**
Create bash script seperti berikut

```sh
#Update system
sudo apt-get update;
sudo apt-get upgrade;
#install nginx
sudo apt install nginx -y;
sleep 2;
#start nginx
sudo service nginx start;
sleep 2;
#check status nginx
sudo service nginx status;
sleep 2;
```
<p aligh="center">
<img src="../Week 2/image task2/bash install nginx.JPG" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

save dengan extension file **nama_File.sh** 
run file dengan menggunakan command

```sh
sh nama_File.sh
```


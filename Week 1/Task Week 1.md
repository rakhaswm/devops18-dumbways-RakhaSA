```sh
Task :
1. Perbedaan antara IP Private & Public, serta IP Dynamic & Static!
2. Buat penjelasan singkat tentang Virtualization!
3. Buat rancangan sebuah jaringan dengan spesifikasi sebagai berikut!
      - CIDR Block : 192.168.1.xxx/24
      - Subnet : 255.255.255.0
      - Gateway : 192.168.1.1
(Gunakan app.diagrams.net untuk membuat diagramnya, Referensi gambar sudah disertakan)
4. Buat step-by-step untuk menginstall Virutal Machine via VMware, Virtualbox atau VM pilihan kalian!
```
Answer :

# 1. 
**Perbedaan IP Privat & Public**
IP Private	IP Public
- Hanya dapat komukasi antar jaringan lokal	Dapat komunikasi diluar jaringan lokal (internet)
- IP ditetapkan oleh administrator jaringan/perangkat	IP ditetapkan oleh ISP 
- Tidak teridentifikasi di internet	Teridentifikasi di internet
- Unik dalam jaringan lokal	Unik secara global

**Perbedaan IP Dynamic & Static**
IP Dynamic	IP Static
- IP ditetapkan oleh server DHCP	IP ditetapkan oleh ISP
- Gratis	Berbayar
- Dapat berubah-ubah	Tidak berubah
- Biasa digunakan oleh rumahan dan kantor	Biasa digunakan oleh bisnis

# 2. **Virtualization** merupakan sebuah teknologi untuk membagi resource yang besar menjadi lebih kecil dan terdapat Hypervisor yang digunakan untuk membuat dan menjalankan virtual machine. 
Kelebihan : 
- kemudahan backup dan recovery 
- kemudahan deployment (dapat clone sebanyak mungkin dengan konfigurasi system yang sama
- dapat memindahkan virtual machine ke server lain jika terjadi kerusahan hardware.

# 3. 
**Rancangan jaringan spesifikasi**
- CIDR Block : 192.168.1.xxx/24
- Subnet : 255.255.255.0
- Gateway : 192.168.1.1

<p align="center">
<img src="../Week 1/Rancangan Jaringan.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

# 4. 
**Step menginstall Virtual Machine dengan VM Ware (OS UBUNTU SERVER)**
**INSTALLATION UBUNTU SERVER**
1.	Buka Virtual Machine dan klik Create a New Virtual Machine. Lalu nanti akan masuk seperti pada gambar ini dan pilih use ISO image, masukan file ISO Ubuntu serter yang sudah didownload sebelumnya.

<p align="center">
<img src="../assets/image/3. OS & Linux/A.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

2.	Masukan user dan password yang di inginkan. Dan ini akan digunakan setiap login Operating System.

<p align="center">
<img src="../assets/image/3. OS & Linux/B.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 
4.	Tentukan lokasi dimana Virtual Machine akan disimpan.

<p align="center">
<img src="../assets/image/3. OS & Linux/C.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

5.	Setelah itu atur size disk yang ingin digunakan. Ada 2 pilihan yaitu Store Disk as Single File dan Split Virtual Disk into Multiple Files.
-	Store Disk as a single file : disk yang akan dicreate langsung terbuat sesuai dengan yang kita inginkan(tidak disarankan pada user yang memiliki kapasitas hardisk kecil)
-	Split virtual disk into multiple files : disk yang digunakan untuk virtual machine nanti akan dibagi menjadi beberapa bagian. (disk yang di set tidak terpakai secara keseluruhan)

<p align="center">
<img src="../assets/image/3. OS & Linux/D.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

5.	Sekarang lakukan customisasi hardware untuk server kita, tekan Customize Hardware.

<p align="center">
<img src="../assets/image/3. OS & Linux/E.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

6.	Terdapat beberapa pilihan untuk melakukan customisasi memory, prosessor dan network adapter.
-	Memory : berfungsi untuk melakukan penyimpanan data yang kita inginkan untuk VM yang kita buat. 
-	Processor : berfungsi untuk memproses data dan mengontrol system yang ada pada VM kita.
-	Network adapter : berfungsi untuk menghubungkan computer ke jaringan.

<p align="center">
<img src="../assets/image/3. OS & Linux/F.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
<img src="../assets/image/3. OS & Linux/G.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 
7.	Jika sudah melakukan setting memory dan proses. Dapat dilanjutkan setting bagian Network Adapter. Setelah itu ubah dari default NAT menjadi Bridge.
-	NAT : IP sudah tersedia oleh VM yang dibuat
-	Bridge : Server yang dibuat mendapatkan internet dari yang kita gunakan.

<p align="center">
<img src="../assets/image/3. OS & Linux/H.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 
8.	Jika sudah klik Finish.

<p align="center">
<img src="../assets/image/3. OS & Linux/I.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

10.	Lalu klik Finish nanti akan langsung diarahkan ke bagian instalasi.

<p align="center">
<img src="../assets/image/3. OS & Linux/J.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 
11.	Tunggu loading hingga prosesnya selesai.
 
12.	Jika sudah muncul tampilan seperti ini, silahkan pilih Bahasa yang ingin digunakan. Contoh English. Lalu pilih Done

<p align="center">
<img src="../assets/image/3. OS & Linux/L.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 
13.	Lalu skip dengan klik Done proses dibawah ini.
 
<p align="center">
<img src="../assets/image/3. OS & Linux/M.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
 <img src="../assets/image/3. OS & Linux/N.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>


14.	Selanjutnya ubah konfigurasi network connection dari DHCPv4 menjadi static.
-	DHCP (Dynamic Host Protocol Configuration) : alamat IP yang berubah pada perangkat yang tersambung pada jaringan tersebut (otomatis)
-	Static : alamat IP yang tidak berubah dari yang setelah diberiakn oleh administrator (manual)

<p align="center">
<img src="../assets/image/3. OS & Linux/P.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 
14.	Pilih bagian ens33 dan masuk pada bagian IPv4 Method dari automatic menjadi manual. 
-	Subnet : istilah teknolog informasi yang membedakan Nework ID dan Host ID. Sebagai penentu porsi Network ID dan Host ID pada deretan kode Biner
-	Address : alamat IP yang digunakan untuk VM yang dibuat 
-	Gateway : berfungsi untuk mengkoneksikan jaringan computer kedalam jaringan lain.
-	Name Servers : masukan IP DNS dari google agar dapat terhubung browser.

<p align="center">
<img src="../assets/image/3. OS & Linux/Q.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>


15.	Lanjutkan tahap selanjutnya klik Done

<p align="center">
<img src="../assets/image/3. OS & Linux/R.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
<img src="../assets/image/3. OS & Linux/S.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

 
16.	Lakukan custom storage layout dan klik Done

<p align="center">
<img src="../assets/image/3. OS & Linux/T.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

17.	Buat 2 partisi untuk Root dan Swap. Pilih Free Space dan pilih Add GPT Partition.
-	Root : sebagai tempat system terinstall
-	Swab : sebagai memory cadangan yang digunakan untuk server kita apabila memory utama penuh
 
<p align="center">
<img src="../assets/image/3. OS & Linux/U.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 

18.	Jika sudah selesai membuat 2 partisi Root dan Swap lakukan klik Done
 
<p align="center">
<img src="../assets/image/3. OS & Linux/V.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

19.	Masukan informasi seperti nama, user, dan password untuk server yang akan dibuat. Dan selanjutnya klik Done

<p align="center">
<img src="../assets/image/3. OS & Linux/W.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 

20.	Checklist install OpenSSG server untuk meremote server yang kita buat.

<p align="center">
<img src="../assets/image/3. OS & Linux/X.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

21.	Lanjutkan ke tahap selanjutnya dan klik Done.

<p align="center">
<img src="../assets/image/3. OS & Linux/Y.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
<img src="../assets/image/3. OS & Linux/Z.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>
 

22.	Jika tahapan instalasi sudah selesai masukan ID dan password yang sudah ter set up. Dan dapat lakukan test server apakah sudah terhubung dalam internet dengan perintah ping 8.8.8.8 (8.8.8.8 / 8.8.4.4 IP DNS google.com)
 `
<p align="center">
<img src="../assets/image/3. OS & Linux/AA.png" alt="Alt text" title="Client - Server" style="display: inline-block; margin: 0 auto;  max-width: 300px ">
</p>

 


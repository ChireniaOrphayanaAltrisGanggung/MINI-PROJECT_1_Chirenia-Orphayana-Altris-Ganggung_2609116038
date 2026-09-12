# MINI-PROJECT_1_Chirenia-Orphayana-Altris-Ganggung_2609116038

PENJELASAN PROGRAM :

Program ini mengenai Pengelolaan Jadwal Keberangkatan Bus Cendana Travel Balikpapan. Program ini digunakan untuk mengelola data jadwal keberangkatan bus dalam periode tanggal 14 - 20 September 2026 (Jadwal keluar setiap Satu Minggu sekali)

Program menggunakan bahasa pemograman Python dan menerapkan konsep dasar seperti List, While, Conditional Satement, Percabangan, Input dan Output.
1. Menampilkan Nama dan Informasi Jadwal Travel

   Pada bagian awal program terdapat perintah print() untuk menampilkan nama program,
   periode jadwal dan informasi mengenai jadwal keberangkatan ketika program pertama
   kali di jalankan oleh user.
   <img width="719" height="142" alt="image" src="https://github.com/user-attachments/assets/261ef893-deec-42c5-910e-d559d93876ea" />

   OUTPUT PROGRAM :
   
   <img width="594" height="135" alt="image" src="https://github.com/user-attachments/assets/8ff68173-4d14-4e2d-984e-cba5bf6b0ca2" />

2. Membuat dan Menampilkan List Jadwal Travel

   Semua jadwal di simpan dalam list dengan nama Jadwal_Travel yang terdiri dari 5 item, yaitu :
   
   jadwal [0] : Hari
   
   jadwal [1] : Jam
   
   jadwal [2] : Rute
   
   jadwal [3] : Mobil
   
   jadwal [4] : Driver
   
   Dengan urutan [Hari, Jam, Rute, Mobil, Driver] data di simpan di dalam list untuk  periode dalam 1 minggu akan di tampilkan di awal bersama dengan nama dan informasi program sebelum user memasuki pilihan menu.
   <img width="762" height="359" alt="image" src="https://github.com/user-attachments/assets/e8a79152-c21e-4d1f-8d76-a9c99f5591b9" />

   OUTPUT PROGRAM :

   <img width="1013" height="296" alt="image" src="https://github.com/user-attachments/assets/0dee4493-c1bc-47f2-b6e5-28da0d7cbeb0" />

3. Perulangan Menu Utama

   Setelah jadwal awal dibuat, program menggunakan "while True" untuk membuat menu utama terus berulang(looping) sehingga user dapat memilih dan menggunakan beberapa menu secara
   berulang kali. Menu - Menu tersebut yaitu :
   1. Menu 1 : Tambah Jadwal
   2. Menu 2 : Ubah Jadwal
   3. Menu 3 : Hapus Jadwal
   4. Menu 4 : Tampilkan Jadwal
   5. Menu 5 : Keluar
      
   Program akan berhenti ketika user memilih menu '5. Keluar' untuk mengakhiri program. Pilihan menu di simpan dalam PILIH_MENU =input(1 - 5) :"). pilihan menu akan selalu muncul ketika
   user kembali ke menu utama, user hanya bisa memilih menu 1 - 5.

   Terdapat Validasi Looping jika user memilih menu lain (6,7 atau huruf abc) maka program akan menampilkan "Pilihan menu tidak tersedia, silahkan
   pilih 1-5" dan meminta user untuk memasukan ulang hingga sesuai pilihan

   <img width="629" height="264" alt="image" src="https://github.com/user-attachments/assets/57e7ed28-849d-4446-9a58-a490d069d379" />

   Program jika pilihan menu tidak tersedia :

   <img width="629" height="104" alt="image" src="https://github.com/user-attachments/assets/50c05394-9d84-4556-9960-3060537aff4e" />

   OUTPUT PROGRAM :

   <img width="261" height="174" alt="image" src="https://github.com/user-attachments/assets/606b6d69-9569-4922-9d25-88f5e57e0c88" />

   OUTPUT PROGRAM JIKA PILIHAN TIDAK TERSEDIA :

   <img width="557" height="331" alt="image" src="https://github.com/user-attachments/assets/0bbec9c2-ea75-4aa8-a9fe-817b33cfeca9" />

4. MANAMBAHKAN JADWAL : MENU 1

   Menu 1 digunakan untuk menambahkan jadwal baru, program akan meminta user memasukan
   5 item yaitu Hari, Jam, Rute, Plat Mobil, Driver yang kemudian akan digabungkan
   menjadi satu dalam list Jadwal_Baru. Item atau data baru akan dimasukan ke dalam
   Jadwal_Travel menggunakan Jadwal_Travel.append(Jadwal_Baru). Disini "append()"
   berfungsi untuk menambahkan jadwal baru ke bagian akhir list. Jika berhasil
   ditambahkan, program akan menampilkan "Jadwal baru berhasil di tambahkan"

   Pada bagian ini juga terdapat "continue" berfungsi kembali ke awal perulangan Menu
   Utama setelah user menggunakan menu 1.

   <img width="678" height="257" alt="image" src="https://github.com/user-attachments/assets/61bf878a-0dd5-4441-9f67-cdff0fedbfa2" />
 

     OUTPUT PROGRAM :

   <img width="1011" height="321" alt="image" src="https://github.com/user-attachments/assets/6dd6775e-43c0-4d23-a551-1eb7d559dcd2" />

5. MENGUBAH JADWAL : MENU 2

   Menu 2 digunakan untuk mengubah jadwal yang sudah ada, biasanya mengubah item di
   dalam jadwal seeperti hari, jam, dll. Dibagian awal, program akan meminta user
   memasukan hari yang ingin diubah dengan Cari_Jadwal = input("Jadwal hari apa yang
   ingin anda ubah? (Berupa nama hari secara lengkap, ex : Senin A").lower(). Pada
   bagian ini, lower() digunakan untuk mengubah input menjadi huruf kecil sehingga
   data tidak memperhatikan besar atau kecilnya huruf.

   Program kemudian membuat variabel : 'ada_jadwal = False' digunakan sebagai penanda apakah jadwal yang di cari ditemukan atau tidak. Program juga menggunakan perulangan 'for' untuk memeriksa setiap item jadwal yang terdapat di dalam list Jadwal_Travel. jika jadwal di temukan, maka 'ada_jadwal = True' sehingga program menampilkan jadwal yang ditemukan. User kemudian bisa memilih bagian yang di ubah tergantung item di dalam jadwal, misalnya user memilih jam : Jadwal[1] = input("Jam Baru :") item pada index 1 akan di ganti dengan item baru. Program kemudian menampilkan Jadwal_Travel yang sudah di perbarui.

   Untuk keluar dari menu dan kembali ke menu utama, user bisa memilih "Selesai" dan jika jadwal tidak ditemukan maka program meminta user untuk menginput kembali hingga sesuai pilihan item dengan menampilkan "Jadwal tidak ditemukan, mohon periksa kembali."

   <img width="939" height="570" alt="image" src="https://github.com/user-attachments/assets/fabbfaa2-8381-4028-bc27-79707593b3ba" />

   <img width="851" height="391" alt="image" src="https://github.com/user-attachments/assets/2e62417a-9225-402b-b678-4436a2b61355" />

   OUTPUT PROGRAM :

   <img width="1029" height="405" alt="image" src="https://github.com/user-attachments/assets/c6b1e976-8563-439b-89bf-f36b1b43081b" />

   OUTPUT PROGRAM JIKA PILIHAN ITEM TIDAK TERSEDIA :
   <img width="858" height="49" alt="image" src="https://github.com/user-attachments/assets/82cd70ae-f3f7-4680-8ec5-2f94041524f5" />
   <img width="831" height="89" alt="image" src="https://github.com/user-attachments/assets/2fdbf5ed-d59e-40a9-9d3d-f5d102bccbd9" />

6. MENGHAPUS JADWAL : MENU 3

   Menu 3 digunakan untuk menghapus jadwal yang terdapat di dalam list, sama seperti sebelumnya program akan meminta user mencari berdasarkan hari. Kemudian program menggunakan variabel
   penanda :

   ditemukan - False
   Hapus_berhasil = False
   "ditemukan" berfungsi untuk mengetahui apakah jadwal yang dicari ditemukan, sedangkan Hapus_berhasil berfungsi untuk mengetahui apakah hapus jadwal berhasil atau tidak. Program mencari jadwal dengan menggunakan 'for jadwal in Jadwal_Travel :' jika jadwal ditemukan, maka program akan menampilkan dan meminta konfirmasi user "Apakah yakin ingin menghapus jadwal ini (ya/tidak)"

   Jika user memilih 'ya' maka data akan dihapus menggunakan Jadwal_Travel.remove(jadwal), 'remove()' digunakan untuk menghapus data tertentu di dalam list. jika berhasil di hapus maka program menampilkan print "Jadwal berhasil di hapus" dan menampilkan Jadwal Travel baru.

   Jika user memilih 'tidak' maka data tidak dihapus dan program menampilkan "Jadwal tidak jadi dihapus" sedangkan jika user memasukan pilihan lain, program akan menampilkan bahwa pilihan tidak tersedia dan user harus memilih antara ya atau tidak.

<img width="920" height="560" alt="image" src="https://github.com/user-attachments/assets/183f6724-5eb5-406b-87b6-c62a62bafbdb" />

  
<img width="809" height="399" alt="image" src="https://github.com/user-attachments/assets/4092cbe8-9e2a-4b62-9f16-2c8b55dc3142" />

OUTPUT PROGRAM : 

<img width="1015" height="345" alt="image" src="https://github.com/user-attachments/assets/ffd79a52-d77c-49c3-b4ef-11cf24d20b10" />

OUTPUT PROGRAM JIKA USER MEMILIH 'TIDAK' :

<img width="901" height="128" alt="image" src="https://github.com/user-attachments/assets/67ca9ac6-d2e6-4dbb-9c04-ed94f4758aa3" />

OUTPUT PROGRAM JIKA USER MEMILIH PILIHAN LAIN :

<img width="869" height="158" alt="image" src="https://github.com/user-attachments/assets/fed0abd7-4081-45c8-a8af-e4ce215aaf4a" />

7. MENAMPILKAN SEMUA JADWAL : MENU 4

   Menu 4 digunakan untuk menampilkan seluruh jadwal yang ada di dalam Jadwal_Travel, program menggunakan perulangan 'for jadwal in Jadwal_Travel:' untuk mengambil dan menampilkan setiap satu per satu jadwal. Agar terlihat rapi, program menampilkan jadwal menggunakan index atau item dari atas ke bawah dan di batasi dengan garis sehingga terlihat lebih terstruktur.
   Program juga menggunakan continue untuk kembali ke menu utama.

   <img width="608" height="330" alt="image" src="https://github.com/user-attachments/assets/75d65eda-5296-49bc-adbd-2c8fa598127b" />

   OUTPUT PROGRAM :

   <img width="492" height="517" alt="image" src="https://github.com/user-attachments/assets/3bbb88e6-b6c6-4ffb-a839-78f92e33aa2b" />

8. MENGAKHIRI PROGRAM (KELUAR) : MENU 5

   Menu 5 digunakan untuk mengakhiri program. Sebelum keluar, program akan meminta konfirasi kepada user "Apakah anda yakin ingin keluar (Ya?Tidak?)

   Jika memilih 'ya' maka user akan keluar dan program menampilkan print "Anda Keluar.", program akan menjalankan 'break' untuk menghentikan perulangan 'while True' di menu utama agar program selesai di jalankan.

   Jika user memilih 'tidak' maka program menampilkan print "Anda kembali ke menu utama" dan menggunakan 'continue' untuk kembali ke menu utama. Sedangkan jika pilihan tidak sesuai, program akan menampilkan bahwa pilihan tidak tersedia dan user harus memilih antara ya atau tidak.

   <img width="833" height="289" alt="image" src="https://github.com/user-attachments/assets/a3ee8084-0ff3-4539-92b3-c4e5775b7636" />

   OUTPUT PROGRAM :

   <img width="432" height="73" alt="image" src="https://github.com/user-attachments/assets/d5056f97-d05f-40b0-9c5a-9724dd379848" />

   OUTPUT PROGRAM JIKA USER MEMILIH 'TIDAK' :

   <img width="522" height="202" alt="image" src="https://github.com/user-attachments/assets/2d594ea0-1770-4017-870b-4135bfa7dc90" />


   OUTPUT PROGRAM JIKA USER MEMILIH PILIHAN LAIN :

   <img width="470" height="69" alt="image" src="https://github.com/user-attachments/assets/d69bd36b-cf3c-4a23-b835-3b182d4e5367" />

OUTPUT PROGRAM KESELURUHAN :
<img width="1021" height="550" alt="image" src="https://github.com/user-attachments/assets/f97d0997-5c00-4660-a3fe-618da919a1dd" />
<img width="1010" height="583" alt="image" src="https://github.com/user-attachments/assets/dd3ebce4-f81d-4c99-acb4-451b56aaa280" />
<img width="1028" height="585" alt="image" src="https://github.com/user-attachments/assets/992cd2f9-65d4-41f7-a461-ac0b112e67f5" />
<img width="1020" height="597" alt="image" src="https://github.com/user-attachments/assets/f4c0bd5c-60b4-4a1b-a055-bd407d09c06e" />
<img width="1021" height="625" alt="image" src="https://github.com/user-attachments/assets/071422fd-590f-49a3-822a-ec07a4ce48ba" />
<img width="1012" height="625" alt="image" src="https://github.com/user-attachments/assets/1d12b90d-22d2-4bfd-80f9-6568a54faddd" />











   


# PRAKTIKUM MODUL 01 KOMUNIKASI DATA DAN JARINGAN KOMPUTER
## Kelompok IT02
### Anggota Kelompok :
|             Nama              |     NRP    |
|-------------------------------|------------|
| Gallant Damas Hayuaji         | 5027231037 |
| Danar Bagus Rasendriya        | 5027231055 |

#### Advance Sanity Check
![image](https://github.com/user-attachments/assets/cd807fba-bbf3-4ed7-9d9b-4e8d97c2f5ea)

Apa username pengirim? ```JaneD03```.

Untuk menemukan username, berikut adalah proses filternya menggunakan ```http.request.method == "POST"``` lalu follow paket berikut

![image](https://github.com/user-attachments/assets/a678f5a6-9d02-4ee2-bb2f-4520e90b8a4a)

![image](https://github.com/user-attachments/assets/5c1114ed-7d89-42e4-8cd6-8fb5e1b43663)

Apa Nama File yang dikirim? ```Clue3.txt```. Didapatkan dari filter "http"

![Screenshot 2024-09-19 004148](https://github.com/user-attachments/assets/df275960-725f-484b-94fc-1ef777b31930)

lalu follow HTTP Stream dan ditemukan file Clue3.txt

![image](https://github.com/user-attachments/assets/b69bba2e-79de-4f8d-ade6-0461ca9f7156)

Lalu mengikuti petunjuk pada ppt peraturan praktikum dan menemukan text berikut ini

![image](https://github.com/user-attachments/assets/103c0b23-973f-4c60-a825-c37de4635f90)

Text tersebut perlu di-decode dengan Base64, menjadi seperti berikut:

![image](https://github.com/user-attachments/assets/887ea428-775c-490a-9cc6-53d61568e198)

Menjadi jawaban pertanyaan 
Ikuti petunjuk untuk mendapatkan pesan rahasia. Kemudian flag didapatkan
Flag: JarkomIT{8uK4n_S4n1ty_b1a5A_fQe1rmHCeu1QqtJM6Xq5jTuJ9Su5BTWwLQd0qPjRxfveVtS3O8h0UIKK}

### Pegawai Negeri Sebelah
![Screenshot (248)](https://github.com/user-attachments/assets/f16424d4-f5b8-4683-867f-ff87e3a0ca29)

Pertama kita mencari nama file dan ditemukan ```data_pns.csv```. File ini akan diexport dan nanti bisa dibaca isinya lewat excel.

![image](https://github.com/user-attachments/assets/0b491208-3dbc-456b-8544-cab85ae589a8)

![image](https://github.com/user-attachments/assets/109fef1b-1a5e-49a4-b1fe-2bb4828748fd)

Setelah itu membuka file di excel dan memasukkan sesuai kebutuhan pertanyaan.

![image](https://github.com/user-attachments/assets/bd5dcfb6-3a2e-4eb0-8c39-8943fcb6a27e)

Flag: JarkomIT{Tum8eN_p45SnYa_Ku4t_B1aS4Nya_X27HTdzty5QRXrCJPeXTXOfSEL37jegV6lQaModIofD8iGf6fTRmM4h}

### FTP Login
![image](https://github.com/user-attachments/assets/480f85df-107e-4977-9047-7a110f7ac35a)\

Apa username yang berhasil digunakan untuk login? ```sn34ky``` . Ini didapatkan dengan cara filter ```ftp.response.code == 230``` untuk menemukan yang berhasil, karena 230 menunjukkan login success.

![image](https://github.com/user-attachments/assets/ea9a95ae-5737-4e18-9e0f-622e09b3feee)

![image](https://github.com/user-attachments/assets/571ebdab-81ad-4e80-ada1-c536d2c96430)

Lalu ditemukan password ```sup3rsn1ff3r```. Kemudian flag ditemukan

### Surprise
![image](https://github.com/user-attachments/assets/ac9c8617-eb8b-4d35-a779-d0479af0f199)

Langkah pertama adalah filtering untuk menemukan nama service yang digunakan sebagai berikut

![image](https://github.com/user-attachments/assets/f6c8fe80-15c6-44d6-89c6-b15302ef082a)

Lalu mencari nama file dengan filter sebagai berikut

![image](https://github.com/user-attachments/assets/f92aeb97-ab40-4055-b678-1cc0b237c1b6)

Untuk menemukan pesan rahasia, saya membuka file ```.cpp``` yang ada dan menemukan kumpulan angka sebagai berikut.

![image](https://github.com/user-attachments/assets/a273d69b-b988-406f-9ef4-f029b7d9a02a)

Angka tersebut perlu dikonversi dari ASCII menjadi text dan didapatkan hasil berikut ini:

![Screenshot 2024-09-18 205750](https://github.com/user-attachments/assets/ef2ba6fb-2507-4d8d-9a74-b13896e68e70)

Sebelumnya saya mengalami beberapa kendala karena salah memasukkan pesan (terdapat ```spasi``` yang membuat salah).

![image](https://github.com/user-attachments/assets/0c3f6953-906c-4139-9be0-032455175444)

### Corporate Breach

Flag yang didapat:

![Screenshot 2024-09-18 at 20 37 20](https://github.com/user-attachments/assets/0ae967a5-f931-4014-9752-6f591ceb6f73)

Pertama saya masuk ke nc soal ini.

Lalu ada pertanyaan:

![image](https://github.com/user-attachments/assets/79110f20-21b5-4298-8962-696d3bd63fbe)

Jawaban: Nakhimov

Saya mendapat jawaban itu dengan melakukan follow-http stream terhadap packet:

![Screenshot 2024-09-19 at 01 35 16](https://github.com/user-attachments/assets/4f1196d8-b8a8-46dd-b5d1-773b13e14535)

Yang menunjukkan string seperti ini:

![Screenshot 2024-09-18 at 20 20 53](https://github.com/user-attachments/assets/f4114fae-5db2-4aa4-8617-93fe481e6efe)

Selanjutnya muncul pertanyaan ke-2:

![Screenshot 2024-09-18 at 20 37 20](https://github.com/user-attachments/assets/4c4832ca-6c25-4173-9284-33ff995d8e2a)

Saya melakukan filtering:

![Screenshot 2024-09-19 at 01 35 16](https://github.com/user-attachments/assets/94ef7bbf-37d1-4fe2-a779-bdc599473519)

Saya cek beberapa packet HTTP dengan info POST dan index.php HTTP/1.1

Lalu saya mendapati email dan password:

![Screenshot 2024-09-18 at 20 36 42](https://github.com/user-attachments/assets/984ad809-c3d5-4a27-ae1e-eca7cf458bc4)

Setelah itu saya input email dan password ke dalam pertanyaan nc, lalu saya mendapatkan flag: JarkomIT{supp0rt_k0k_l3m4h_bg_knHDj2iRrQWdXNOuGb7Mm8EZ6G6HMjbdH7CSz0iuPfDdzUi6iejBG6}

### Soal EZ

Flag yang didapat:

![Screenshot 2024-09-18 at 20 07 24](https://github.com/user-attachments/assets/ce9a4889-ef7c-450c-9947-c4ac84d0b2a2)

Pertanyaan 1: saya dapat dari membuka beberapa file yang menurut saya "berbeda"

![Screenshot 2024-09-19 at 01 52 57](https://github.com/user-attachments/assets/c171d8c8-2212-41ec-8f88-293329901a29)

Lalu saya mendapat:

![Screenshot 2024-09-18 at 20 05 56](https://github.com/user-attachments/assets/8bf6f01f-236b-41a7-b34b-d5ea12d633e0)

Lalu saya cek port dari packet yang saya follow, saya dapatkan nomor port nya:

![Screenshot 2024-09-18 at 20 07 24](https://github.com/user-attachments/assets/72a9c8da-19a6-4cf6-b5a1-bb2e9f698d3f)

Flag pun didapatkan 

-----------------------------------------------------------
## Pengerjaan Revisi Modul 1
### Soal Illegal Breakthrough

![image](https://github.com/user-attachments/assets/47d9a04b-8a92-4140-8229-787bba15cd69)
![image](https://github.com/user-attachments/assets/ebaa57f5-fe76-48c9-a818-f11b7755d897)
![image](https://github.com/user-attachments/assets/530ab2b0-b1f6-4cf5-90d6-01106729b4db)

Apa IP Address dari korban? ```172.21.88.207```. Caranya adalah dengan mengecek destination. Di sini dicurigai karena banyak IP yang sama dan waktu yang berdekatan.

![image](https://github.com/user-attachments/assets/d9f2b99e-f106-4ed5-9857-f38a4203d7b7)

Apa port yang digunakan sebagai webserver? ```1917```. Caranya adalah dengan mengecek destination port di bawah.

![image](https://github.com/user-attachments/assets/7a5405ad-d0d3-45e9-b2aa-aa4f1266c531)

Dimana endpoint yang terdapat login? ```/ww1.php```. Dengan cara filtering menggunakan ```frame contains "POST"``` lalu melakukan follow HTTP.

![image](https://github.com/user-attachments/assets/8460101f-408b-445e-8c5c-11abc7a2cc08)

Tools apa yang digunakan oleh attacker? ```ffuf-v2.1.0-dev```. Nama asli dari tools bisa ditemukan bersamaan dengan endpoint di atas. Nama tools ```Fuzz Faster U Fool```, tetapi di sini perlu disingkat.

Apa Kredensial yang berhasil digunakan oleh attacker untuk login? ```Redbaron:fly1ng4c3```. Untuk menemukannya bisa menggunakan filter ```frame contains "password"```

![image](https://github.com/user-attachments/assets/c09a46bd-1560-4e3c-95a5-2490d2d0ebe2)
![image](https://github.com/user-attachments/assets/6ef6c9ec-576b-4a13-ac12-3e9a3792cc9f)

Flag: ```JarkomIT{d34th_fr0m_th3_sky_gnavhIKKBQrJEfvUIfmkReZOCH1aR8ZIwidUScBKcbmxCdRONEXLWW1}```

### Soal Packets Barrage
![image](https://github.com/user-attachments/assets/1f168e47-04ba-47c1-b728-ac0014b6fbb0)
![image](https://github.com/user-attachments/assets/a296faee-93fa-4c54-9781-3efca9a8813a)
![image](https://github.com/user-attachments/assets/68e6bf78-74ad-44c3-a529-8d7c413236d3)
![image](https://github.com/user-attachments/assets/2299c59b-1b21-4efa-b4c2-5919908fa248)

Apa IP address dari attacker? ```172.21.80.1```. Melakukan filtering ```http``` dan melihat IP yang menuju ke korban.

![image](https://github.com/user-attachments/assets/86a9dce6-037c-4959-b633-0590b545b8d3)

Berapa total attempt dari bruteforce attacker? ```1917```. Filtering response ```ip.dst == 172.21.88.207 && http.request.method == "POST"``` yang mengarah ke IP korban.

![image](https://github.com/user-attachments/assets/96d8fdb8-8cba-4d87-a13f-18287fc82939)
![image](https://github.com/user-attachments/assets/796dab61-1d6d-4abc-aaa5-7c44a1099b20)

Apa nama file yang didownload oleh attacker setelah berhasil login ```Albatros.txt```. Filter ```ip.src == 172.21.80.1 && http.request.method == "GET"``` untuk melihat request ```GET``` yang dilakukan attacker. Lalu follow HTTP stream pada paket.

![image](https://github.com/user-attachments/assets/f9b34cb8-c3e7-4eac-906f-8766833c330f)
![image](https://github.com/user-attachments/assets/32a80427-9d17-44e1-9aa2-ee9a5df4252d)

Apa isi dari file yang disisipkan oleh attacker? ```Der Rote Kampfflieger```. Membuka file ```break.pcapng``` di Visual Studio Code dan mencari Albatros.

![image](https://github.com/user-attachments/assets/98c259af-30da-4d49-8132-19a1adf71561)

Flag: JarkomIT{th3_fly1ng_c1rcus_0f_w4r_gownfDVvIIiaBPo1fFhviboDH5StXEHd7pnMuDlkxgdZgnsxELzzjACE}

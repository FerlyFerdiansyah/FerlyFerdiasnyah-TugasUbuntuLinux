Soal dan Jawabannya ;
1. Eksekusi seluruh profile yang ada :  
  a.	Edit file profile /etc/profile dan tampilkan pesan sebagai berikut :  
    echo “Profile dari /etc/profile”
![VirtualBox_ubuntu_25_09_2024_21_08_07](https://github.com/user-attachments/assets/be1b5d1f-3ae2-4fd0-9e8c-16d92ceeb5d6)

![VirtualBox_ubuntu_25_09_2024_22_15_08](https://github.com/user-attachments/assets/9d710613-3e76-4158-bc21-1c69ffce376e)


  b.	Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu :  
    /home/stD02001/.bash_profile  
    /home/. stD02001/.bash_login  
    /home/mahasiswa/.profile  /home/mahasiswa/.bashrc  
    Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap  file tersebut, cantumkan instruksi echo, misalnya pada /home/ mahasiswa/.bash_profile :  
    echo “Profile dari .bash_profile”  
    Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.
![VirtualBox_ubuntu_25_09_2024_23_03_27](https://github.com/user-attachments/assets/e733e641-2ba0-41b8-9d7c-626815ba1f28)

![VirtualBox_ubuntu_25_09_2024_23_08_45](https://github.com/user-attachments/assets/64d63893-4554-47e0-8d07-8c3e1a50dbdd)

![VirtualBox_ubuntu_25_09_2024_23_14_58](https://github.com/user-attachments/assets/c0dbe963-c3d6-4ce8-b030-5a0ec4285fb2)

![VirtualBox_ubuntu_25_09_2024_23_18_45](https://github.com/user-attachments/assets/7e85b53c-84c0-4deb-98db-b3df30a23ab1)

![VirtualBox_ubuntu_25_09_2024_23_31_30](https://github.com/user-attachments/assets/35c4ae6f-d6e1-4434-ae55-4e7812788939)

  c.	Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:  
    $ su mahasiswa  
    $ exit  
![VirtualBox_ubuntu_25_09_2024_23_35_50](https://github.com/user-attachments/assets/81e7a987-d8e1-4634-901c-4b8dc927ed1d)

    kemudian gunakan opsi – sebagai berikut :  
    $ su – mahasiswa  
    $ exit  
![VirtualBox_ubuntu_25_09_2024_23_36_59](https://github.com/user-attachments/assets/820fbbce-4734-4498-9202-28c42b683573)

    
    Jelaskan perbedaan kedua utilitas tersebut.
    "Perbedaan kedua utilitas tersebut yaitu adanya permintaan password pada opsi syntax kedua, 
    menampilkan isi dari file-file yang dibuat pada direktori yang berbeda. 
    Untuk direktori yang memiliki banyak file, hanya akan ditampilkan satu buah filenya saja."

2. Prompt String (PS)  
  a.	Edit file .bash_profile, ganti prompt PS1 dengan ‘>’. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell  
    PS1=‟> „
     export PS1.
  b.	Eksperimen hasil PS1 :  
    $ PS1=“\! > “  
    69 > PS1=”\d > “  
    Mon Sep 23 > PS1=”\t > “  
    10:10:20 > PS1=”Saya=\u > “  
    Saya=mahasiswa > PS1=”\w >”  ~ > PS1=\h >”
![VirtualBox_ubuntu_25_09_2024_23_50_28](https://github.com/user-attachments/assets/2f5c78a0-30ac-4928-816d-c4e77cb72a49)

3.	Logout  
  Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout  
  Echo “Terima kasih atas sesi yang diberikan”  Sleep 5  clear
![VirtualBox_ubuntu_26_09_2024_00_12_39](https://github.com/user-attachments/assets/43c2b90c-a9fe-41a4-bf14-c0d2511fa10a)


4.	Bash script  
  a.	Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing :  
    p1.sh  #! /bin/bash  echo “Program p1”  ls –l
  	p2.sh  #! /bin/bash  echo “Program p2”  who
  	p3.sh  #! /bin/bash  echo “Program p3”  ps x
![VirtualBox_ubuntu_26_09_2024_00_32_03](https://github.com/user-attachments/assets/767ca9d0-00f7-410f-8423-b0e126536413)

![VirtualBox_ubuntu_26_09_2024_00_32_26](https://github.com/user-attachments/assets/df492537-25fb-410b-af65-2c5784a693ee)

![VirtualBox_ubuntu_26_09_2024_00_32_43](https://github.com/user-attachments/assets/e528eb6c-cb1a-4a09-9a7c-6da4eec35b20)

  b.	Jalankan script tersebut sebagai berikut :  
    $  ./p1.sh ; ./p3.sh ; ./p2.sh  
    $  ./p1.sh &  
    $  ./p1.sh $ ./p2.sh & ./p3.sh &  
    $  ( ./p1.sh ; ./p3.sh ) &  
![VirtualBox_ubuntu_26_09_2024_00_41_32](https://github.com/user-attachments/assets/a98ef2ea-1b1e-453d-be5b-3316892b7500)

![VirtualBox_ubuntu_26_09_2024_00_43_01](https://github.com/user-attachments/assets/eff58624-3a35-43be-9a2a-18422f82d307)

![VirtualBox_ubuntu_26_09_2024_00_44_56](https://github.com/user-attachments/assets/f9514fc6-d62c-49e7-bd23-e96ca8cca982)

![VirtualBox_ubuntu_26_09_2024_00_47_17](https://github.com/user-attachments/assets/c086165d-41e9-4425-a0b5-ba1101e8cc3c)


5. Jobs  
  a.	Buat shell-script yang melakukan loop dengan nama pwaktu.sh,  setiap 10 detik,
  kemudian menyimpan tanggal dan jam pada file hasil.  #!/bin/bash  while [ true ]  do   date >> hasil   sleep 10  done  
![VirtualBox_ubuntu_26_09_2024_00_58_51](https://github.com/user-attachments/assets/01c55326-d54d-41ae-aa95-6296752b4c82)


  b.	Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut :  
    $ jobs  
    $ find / -print > files 2>/dev/null &  
    $ jobs  
![VirtualBox_ubuntu_26_09_2024_01_04_36](https://github.com/user-attachments/assets/d0812f36-109f-40e7-b889-4f382e847836)


  c.	Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background  
    $ fg %1  
    $ bg  
![VirtualBox_ubuntu_26_09_2024_01_09_25](https://github.com/user-attachments/assets/181d59b0-b596-4502-b3d5-29bbd3bb480d)


  d.	Stop program background dengan utilitas kil  
    $ ps x  
    $ kill [Nomor PID]  
![VirtualBox_ubuntu_26_09_2024_01_10_22](https://github.com/user-attachments/assets/7eeab54c-854e-41a7-bb80-04e12f1b2820)

![VirtualBox_ubuntu_26_09_2024_01_12_37](https://github.com/user-attachments/assets/3541a005-a39d-472c-b8fa-df493efa8fdb)


6. History  
  a.	Ganti nilai HISTSIZE dari 1000 menjadi 20  
    $ HITSIZE=20  
    $ h  
![VirtualBox_ubuntu_26_09_2024_01_16_19](https://github.com/user-attachments/assets/5d78f246-b045-48a7-b972-f67f8aafa8a0)


  b.	Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan  
    $ !-5  
![VirtualBox_ubuntu_26_09_2024_01_17_36](https://github.com/user-attachments/assets/581d935f-e57e-4a9c-9a7d-66783b553e63)


  c.	Ulangi instruksi yang terakhir.  Gunakan juga ^P dan ^N untuk bernavigasi pada history buffer  
    $ !!  
![VirtualBox_ubuntu_26_09_2024_01_18_53](https://github.com/user-attachments/assets/0c714378-5cae-4e25-a9fa-35421980f4ff)


Hasil navigasi saat menggunakan ^P maupun ^N pada history buffer
![VirtualBox_ubuntu_26_09_2024_01_20_14](https://github.com/user-attachments/assets/44c05253-5e67-4df9-aa8c-810d7342e44b)


  d.	Ulangi instruksi pada history bufer nomor 150  
    $ !150. Namun karena tidak ada intruksi buffer pada nomor 150, maka saya ganti nomor 158  
![VirtualBox_ubuntu_26_09_2024_01_24_18](https://github.com/user-attachments/assets/2885ea0d-d157-4a2b-b555-d9ed18bb1e50)


  e.	Ulangi instruksi dengan prefix “ls”  
    $ !ls  
![VirtualBox_ubuntu_26_09_2024_01_26_05](https://github.com/user-attachments/assets/303d9e7d-eb5e-48a2-94c8-532f8058364c)




Tugas : Buat 50 Command Line 


![alt text](![VirtualBox_ubuntu_05_09_2024_01_35_57](https://github.com/user-attachments/assets/f98379d6-ade7-42dd-9fa9-fea01016807a)
?raw=true) 

1. lsb_release -a (melihat versi Ubuntu)
2. pwd (melihat directory saat ini)
3. ls (melihat isi directory)
4. mkdir project (membuat direktori baru dengan nama "project")
5. cd project (masuk ke direktori baru)
6. touch tes.txt (membuat file kosong dengan nama "tex.txt")
7. nano tes.txt (membuka file "tes.txt" dengan editor text)
8. echo "hello" > tes.txt (menambahkan teks yakni "Done" ke dalam tes.txt)
9. cat tes.txt (melihat isi file(hanya baris pertama saja yg ditampilkan))
10. cp tes.txt tesno2.txt (menyalin file dari tes.txt ke tesno2.txt)
11. mv tesno2.txt myfile.txt (mengganti nama file dari "tes2.txt" ke "myfile.txt")
12. echo "form2" . dupe.txt (membuat file dan menambah isinya)
13. cat myfile.txt dupe.txt > gabung.txt (menggabungkan dua file menjadi 1 ke dalam file "gabung.txt")
14. rm dupe.txt (menghapus file "dupe.txt")
15. mkdir newfile2(membuat folder baru di dalam folder)
16. myfile.txt newfile2/ (memindahkan file "myfile.txt" ke folder "newfile2")
17. cp -r newfile2/ newfile3/ (menyalin direktori dan isinya dari "newfile2" ke "newfile3")
18. ls -R (melihat isi direktori secara rekursif, yg dimana pada bagian ini melihat direktori "newfile")
19. clear (Untuk membersihkan/mengosongkan terminal)
20. cd .. (untuk keluar satu tingkat dari direktori yg dibuka sebelumnya)



![alt text](![VirtualBox_ubuntu_05_09_2024_01_42_18](https://github.com/user-attachments/assets/b8f32f17-3eb6-4b34-99f5-30fca626c77d)
?raw=true)

21. df -h (melihat penggunaan disk)
22. du -sh project (melihat penggunaan ruang dalam direktori "newfile")
23. ls -a (menampilkan file tersembunyi di direktori)
24. rmdir newfile3 (menghapus direktori kosong, karena newfile3 saya berisi file maka tidak bisa dihapus)
25. rm -r newfile3 (menghapus direktori beserta isinya)
26. chmod +x script.sh (membuat file dengan hak akses tertentu)
27. ./script.sh (menjalankan script bash)
28. ps aux (menampilkan informasi proses yang sedang berjalan pada sistem)



![alt text](?![VirtualBox_ubuntu_05_09_2024_01_50_08](https://github.com/user-attachments/assets/d96f4cc8-543d-49fb-ab8a-95db430ee4af)
raw=true)

29. kill 3806 (membunuh proses yang berjalan berdasarkan nomor PIDD yg di tampilkan pada command ps aux sebelumnya)
30. find . -name "myfile.txt" (mencari file dalam direktori)
31. sudo command_name ("sudo" untuk menjalankan perintah dengan hak akses root)
32. sudo chown ferly-ferdiansyah:ferly-ferdiansyah tes.txt (mengganti kepemilikan file, karena saya hanya memiliki satu user jadi cmn ada name user "ferly-ferdiansyah")
33. sudo apt update (meng-update package list)



![alt text](?![VirtualBox_ubuntu_05_09_2024_01_51_08](https://github.com/user-attachments/assets/dce12bb2-4d42-438c-858b-dbe1b9ee6899)
raw=true)

34. sudo apt upgrade (meng-upgrade sistem)



![alt text](?![VirtualBox_ubuntu_05_09_2024_01_59_32](https://github.com/user-attachments/assets/3e522760-a333-4e6a-badf-94f1c89024b3)
raw=true)

35. sudo apt install vim (menginstall aplikasi)
36. sudo apt remove vim (menghapus aplikasi)
37. sudo apt autoremove (membersihkan package yang tidak terpakai)
38. grep "hello" tes.txt ("grep" untuk mencari teks dalam file)
39. man ls (menampilkan halaman manual dari perintah)
40. wx -l tes.txt (menghitung jumlah baris dalam file)
41. swapon --show (menampilkan ruang swap)



![alt text](![VirtualBox_ubuntu_05_09_2024_02_07_20](https://github.com/user-attachments/assets/bf24c4f7-983f-4748-95b6-45bb8c66714e)
?raw=true)

42. ip add (melihat ip address)



![alt text](![VirtualBox_ubuntu_05_09_2024_02_10_59](https://github.com/user-attachments/assets/59e6af17-ceb2-41e7-a51b-6b1d6449a9b0)
?raw=true)

43. sudo adduser guest (menambahkan user baru yakni "guest")
44. sudo deluser guest (menghapus user guest)



![alt text](![VirtualBox_ubuntu_05_09_2024_02_11_50](https://github.com/user-attachments/assets/42061837-1b89-4217-9180-d9256528ab1c)
?raw=true)

45. sudo lshw -short (menampilkan informasi hardware)



![alt text](![VirtualBox_ubuntu_05_09_2024_02_40_32](https://github.com/user-attachments/assets/0cd16610-47c8-47bd-86bf-dccb3f45955b)
?raw=true)

46. sed (menemukan,mengganti,menghapus pola dalam file)



![alt text](![VirtualBox_ubuntu_05_09_2024_02_41_17](https://github.com/user-attachments/assets/a83bd3b0-ae20-47f8-b763-c34da063ad1a)
?raw=true)

47. file (memeriksa jenis file)



![alt text](![VirtualBox_ubuntu_05_09_2024_03_50_09](https://github.com/user-attachments/assets/9d5116e1-7236-4b6c-8bd4-6b58d45c356c)
?raw=true)

48. dig (menampilkan informasi DNS)
49. top (menampilkan proses yang berjalan dan penggunaan resource sistem)



![alt text](![VirtualBox_ubuntu_05_09_2024_02_55_37](https://github.com/user-attachments/assets/031e9780-90f4-4809-9c60-2c4b9f964cf9)
?raw=true)

50. sudo timedatectl set-timezone Asia/Jakarta (untuk mengatur waktu,tanggal, dan zona waktu)
51. sudo shutdown now (mematikan/men-shutdown sistem)

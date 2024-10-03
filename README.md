  ## Laporan Installasi dan Konfigurasi SSH

</div>

  ### Menyiapkan Ubuntu
  Langkah pertama yang perlu dilakukan adalah mempersiapkan Ubuntu dengan cara :
  - > sudo apt update && apt upgrade
![VirtualBox_Ubuntu22_03_10_2024_00_26_22](https://github.com/user-attachments/assets/6aec41a5-32d5-412b-b570-ce9c52069361)


<br>


  ### Install SSH pada Ubuntu
  jalankan command : 
  - > sudo apt install openssh-server
![VirtualBox_Ubuntu22_03_10_2024_00_27_30](https://github.com/user-attachments/assets/02b31452-f3b6-4515-86f7-d3ae73027055)

    

<br>


  ### Start SSH
  jalankan program SSH pada Ubuntu :
   - > sudo systemctl enable --now ssh
![VirtualBox_Ubuntu22_03_10_2024_00_28_25](https://github.com/user-attachments/assets/321b5da4-e2ac-4371-ba69-737365cc7072)

  Cek Status :
   - > sudo systemctl status ssh
![VirtualBox_Ubuntu22_03_10_2024_00_28_37](https://github.com/user-attachments/assets/91ea7e84-8f81-4dfc-9bda-12a1703fc064)



<br>


  ### Konfigurasi Firewall
  Cek UFW Status :
   - > sudo ufw status
![VirtualBox_Ubuntu22_03_10_2024_00_29_47](https://github.com/user-attachments/assets/de134e06-039a-49ae-b3d0-c799891d5710)


  Jika status UFW inactive seperti di kasus ini, maka kita dapat mengaktifkan dengan:
  - > sudo ufw allow ssh
![VirtualBox_Ubuntu22_03_10_2024_00_30_06](https://github.com/user-attachments/assets/1bfd3c03-5f65-42fb-a874-d685d8edf421)



<br>


  ### Sambungkan ke Server
  Coba sambungkan ke server sendiri dengan user dan ip sendiri
  - > ssh ferlyferdiansyah@192.168.184.218
![VirtualBox_Ubuntu22_03_10_2024_09_46_17](https://github.com/user-attachments/assets/eb0f710b-5018-4c55-a474-87fb31460f65)


  Mencoba untuk connect ke SSH server sendiri melalui Putty
  - > Connect Dari Putty
![Screenshot (7)](https://github.com/user-attachments/assets/6dc73e4c-dcdc-438d-8512-64b03d42ebca)



  

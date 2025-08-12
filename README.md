# LAB-4
Selasa 12 Agustus 2025

# Command Line Interface (CLI) pada Mikrotik 
  Selain GUI, untuk konfig Mikrotik juga bisa mengunakan CLI atau Terminal. Yang dapat di akses di winbox terminal, webfig terminal, putty, dan Mikrotik Pro untuk smartphone. Jika mesih bingung dengan command-commandnya, cukup melihat ke GUI winboxnya, contoh, kita ingin set IP DHCP Client untuk ether1, kita lupa command nya apa, kita tinggal melihat ke GUI saja, IP DHCP Client di GUI ada di  
**IP > DHCP Client**  
berarti commandnya

    ip dhcp-client 
dan untuk menambahkan IP DHCP-Client di GUI  
**IP > DHCP-Client > Add/+ > Interface=ether1 > [V] use peer dns > [V] use peer ntp > add default route=yes > enable [V]**  
berarti kalo di CLI

    ip dhcp-client add interface=ether1 use-peer-dns=yes use-peer-ntp=yes add-default-route=yes disabled=no
Berbeda dengan Terminal Linux dan Windows, di terminal RouterOS, kita bisa menyingkat command, seperti

    ip address print
Bisa disingkat jadi

    ip add pr
    
# Meliat Command yang tersedia
Selain itu, kita juga bisa mengunakan key/tombol **TAB** di keyboard (disamping **Q**) untuk melihat command list/daftar perintah yang bisa digunakan. Jadi jika kita sedang konfigurasi dan lupa lanjutannya, kita cukup tekan **TAB** saja.  
![TAB](TAB.PNG)  
Masih bingung dengan **TAB**? Selain mengunakan **TAB** key, kita juga bisa menggunakan **?** di keyboard (SHIFT + /). Berbeda dengan **TAB** yang hanya melihat command, selain untuk melihat command **?** juga menampilkan penjelasan setiap commandnya. Jadi jika bingung apa sih fungsi dari command ini, kita bisa mengunakan **?** command dan penjelasannya akan muncul.  
![Q](Q.PNG)  
# Beberapa Command dan Penjelasannya
  1. ip address print
![ipp](ippr.PNG)
  Digunakan untuk melihat ip address dan di interface mana ip address itu.
**#** disitu maksudnya Number
**Address** IP Address yang digunakan di interface itu
**Network** IP Network

  3. interface print  
  4. 

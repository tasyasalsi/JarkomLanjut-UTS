# Cased
## Topologi Jaringan
![topologi jarkomm](https://github.com/user-attachments/assets/53520eff-6b51-4e0a-b4c7-144069ad251d)

## Analisa Jaringan
- **Koneksi Antar Kampus:** Koneksi antara KJ dan masing-masing cabang (CR dan KHI) dibuat melalui tunnel VPN (IPSec). Tunnel0 menghubungkan KJ dengan CR, sementara Tunnel1 menghubungkan KJ dengan KHI, memungkinkan transfer data yang aman.
- **Segmentasi VLAN:** Setiap kampus memiliki VLAN khusus untuk jaringan lokalnya, memastikan isolasi trafik lokal antar kampus. VLAN 10 (Lab_Praktikum) di KJ, VLAN 20 (Lab_Praktikum_CR) di CR, dan VLAN 30 (Lab_Praktikum_KHI) di KHI. Pengaturan ini memungkinkan akses yang aman dan tersegmentasi bagi setiap kampus.
- **Rute Statis:** Konfigurasi rute statis pada KJ, CR, dan KHI memastikan bahwa setiap kampus dapat mengakses jaringan internal lainnya melalui IP yang telah ditetapkan pada masing-masing interface Tunnel.

# ESSAY

## 1. Static Routing
Static routing adalah metode pengaturan route yang diatur secara manual. Pada static routing, rute ditentukan dan dikonfigurasi langsung pada perangkat jaringan seperti router.

## 2. Dynamic Routing
Dynamic routing adalah metode routing di mana perangkat jaringan seperti router, secara otomatis menemukan jalur terbaik untuk mengirimkan data.

## 3. Firewall
Firewall adalah sistem keamanan jaringan yang memantau dan mengendalikan lalu lintas jaringan yang masuk dan keluar berdasarkan aturan keamanan yang telah ditentukan. Firewall berfungsi sebagai penghalang antara jaringan internal yang aman dan jaringan eksternal yang dianggap tidak aman. 

## 4. NAT (Network Address Translation)
NAT adalah teknologi jaringan yang memungkinkan pengubahan alamat IP dalam header paket data saat melewati router atau perangkat NAT. NAT biasanya digunakan untuk menghubungkan banyak perangkat dalam jaringan lokal (LAN) ke internet dengan menggunakan satu alamat IP publik.

**Jenis-jenis NAT:**
- **Static NAT:** Mengonversi satu alamat IP lokal ke satu alamat IP publik secara tetap.
- **Dynamic NAT:** Mengonversi beberapa alamat IP lokal ke beberapa alamat IP publik secara dinamis.
- **PAT (Port Address Translation):** Juga dikenal sebagai NAT Overloading.

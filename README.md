# Cased
## Topologi Jaringan
![Topologi KampusS](https://github.com/user-attachments/assets/b0739d09-9764-48fd-a9f8-671fef596f0d)
### Deskripsi Topologi
Jaringan ini melibatkan 3 lokasi yang terhubung menggunakan tunnel. Setiap lokasi memiliki router yang saling terhubung melalui tunnel VPN. Router KJ bertindak sebagai pusat untuk menghubungkan lokasi CR dan KHI.

## Analisa Jaringan
### Rute Antar Kampus
- Kampus Kebon Jeruk (KJ) menghubungkan Kampus Citra Raya (CR) dan Kampus Harapan Indah (KHI) melalui 2 tunnel terpisah:
- **Tunnel0** (IP 10.0.0.1/30) menghubungkan KJ dengan CR.
- **Tunnel1** (IP 10.0.1.1/30) menghubungkan KJ dengan KHI.
Setiap router memiliki rute statis untuk memastikan data yang dikirim menuju tujuan yang tepat.

### Analisis Komunikasi Antar Jaringan
#### 1. CR ke KJ:
- Ketika router CR ingin berkomunikasi dengan KJ, paket akan melewati Tunnel0 yang mengarah ke IP KJ (10.0.0.1).
- KJ menerima paket ini melalui Tunnel0 dan dapat mengarahkan paket ke KHI jika diperlukan.
#### 2. KHI ke KJ:
- Ketika router KHI ingin berkomunikasi dengan KJ, paket akan melewati Tunnel1 yang mengarah ke IP KJ (10.0.1.1).
- KJ menerima paket ini melalui Tunnel1 dan dapat mengarahkan paket ke CR jika diperlukan.
#### 3. CR ke KHI:
- CR mengirimkan paket ke KHI dengan melewati Tunnel0 menuju KJ.
- Setelah sampai di KJ, paket akan diteruskan melalui Tunnel1 ke KHI.
#### 4. KHI ke CR:
- KHI mengirimkan paket ke CR dengan melewati Tunnel1 menuju KJ.
- Setelah sampai di KJ, paket akan diteruskan melalui Tunnel0 ke CR.

### Kesimpulan
Jaringan ini berfungsi untuk menghubungkan KJ dengan CR dan KHI menggunakan Tunnel VPN. KJ bertindak sebagai pusat penghubung yang memungkinkan komunikasi atau pertukaran data antara CR dan KHI dengan tunnel yang terpisah. 

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

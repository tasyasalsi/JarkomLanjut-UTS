# ESSAY

## 1. Static Routing
Static routing adalah metode pengaturan jalur (route) jaringan yang diatur secara manual oleh administrator jaringan. Pada static routing, jalur atau rute ditentukan dan dikonfigurasi langsung pada perangkat jaringan seperti router. Rute-rute ini tidak berubah kecuali ada perubahan manual oleh administrator. Static routing sering digunakan dalam jaringan kecil atau jaringan yang jarang berubah karena lebih stabil dan tidak memerlukan overhead pemrosesan tambahan untuk menentukan jalur.

**Keuntungan Static Routing:**
- Lebih aman, karena tidak ada rute yang didapat secara otomatis.
- Menggunakan sedikit sumber daya karena tidak memerlukan proses perhitungan rute.

**Kelemahan Static Routing:**
- Kurang fleksibel; membutuhkan konfigurasi manual ketika ada perubahan jaringan.
- Tidak skala baik dalam jaringan besar atau dinamis.

## 2. Dynamic Routing
Dynamic routing adalah metode routing di mana perangkat jaringan, seperti router, secara otomatis menemukan jalur terbaik untuk mengirimkan data. Proses ini dilakukan dengan menggunakan protokol routing seperti OSPF (Open Shortest Path First), RIP (Routing Information Protocol), atau BGP (Border Gateway Protocol). Router dapat berkomunikasi satu sama lain untuk menginformasikan rute-rute baru atau perubahan rute, sehingga penyesuaian dapat dilakukan secara otomatis.

**Keuntungan Dynamic Routing:**
- Lebih fleksibel dan dapat beradaptasi dengan perubahan jaringan secara otomatis.
- Lebih skala untuk jaringan besar dengan rute yang kompleks.

**Kelemahan Dynamic Routing:**
- Membutuhkan lebih banyak sumber daya (CPU, memori) karena adanya perhitungan dan pembaruan otomatis.
- Risiko keamanan yang lebih tinggi karena rute dapat berubah secara otomatis berdasarkan informasi dari perangkat lain.

## 3. Firewall
Firewall adalah sistem keamanan jaringan yang memantau dan mengendalikan lalu lintas jaringan yang masuk dan keluar berdasarkan aturan keamanan yang telah ditentukan. Firewall berfungsi sebagai penghalang antara jaringan internal yang aman dan jaringan eksternal yang dianggap tidak aman (seperti internet). Terdapat dua jenis firewall, yaitu firewall perangkat keras dan firewall perangkat lunak, serta beberapa jenis teknik firewall, seperti packet filtering, stateful inspection, dan application-level gateway.

**Fungsi Utama Firewall:**
- Mengamankan jaringan dari ancaman eksternal seperti serangan hacker dan malware.
- Menyaring lalu lintas yang tidak diinginkan atau berbahaya.

## 4. NAT (Network Address Translation)
NAT adalah teknologi jaringan yang memungkinkan pengubahan alamat IP dalam header paket data saat melewati router atau perangkat NAT. NAT biasanya digunakan untuk menghubungkan banyak perangkat dalam jaringan lokal (LAN) ke internet dengan menggunakan satu alamat IP publik. Dengan demikian, NAT membantu menghemat penggunaan alamat IP publik yang terbatas dan meningkatkan keamanan dengan menyembunyikan alamat IP internal dari jaringan publik.

**Jenis-jenis NAT:**
- **Static NAT:** Mengonversi satu alamat IP lokal ke satu alamat IP publik secara tetap.
- **Dynamic NAT:** Mengonversi beberapa alamat IP lokal ke beberapa alamat IP publik secara dinamis.
- **PAT (Port Address Translation):** Juga dikenal sebagai NAT Overloading, di mana beberapa alamat IP lokal diterjemahkan ke satu alamat IP publik dengan perbedaan nomor port.

**Keuntungan NAT:**
- Meningkatkan keamanan jaringan dengan menyembunyikan IP internal.
- Menghemat penggunaan alamat IP publik yang terbatas.

# Cased
## Topologi Jaringan
![WhatsApp Image 2024-11-06 at 09 40 28_4f9afd71](https://github.com/user-attachments/assets/bca08a59-175c-4d0f-8679-e9842036898d)

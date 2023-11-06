## CHAPTER 4 MODUL 4 

## Modul 4: Keamanan AWS Cloud

Keamanan AWS Cloud.Keamanan adalah prioritas tertinggi di Amazon Web Services (AWS). AWS memberikan lingkungan komputasi cloud terukur yang dirancang untuk ketersediaan dan ketergantungan tinggi, sambil menyediakan tool yang memungkinkan Anda menjalankan berbagai aplikasi. Membantu melindungi kerahasiaan, integritas, dan ketersediaan sistem dan data Anda sangat penting bagi AWS, begitu pun dengan menjaga kepercayaan pelanggan.

## Modul ini akan membahas topik-topik berikut:
- Model tanggung jawab bersama AWS
- AWS Identity and Access Management (IAM)
- Mengamankan akun AWS baru•Mengamankan akun
- Mengamankan data di AWS
- Berupaya Memastikan Kepatuhan
- Layanan keamanan dan sumber daya tambahan

## Bagian 1: Model tanggung jawab bersama AWS

Keamanan dan kepatuhan merupakan tanggung jawab bersama antara AWS dan pelanggan. AWS bertanggung jawab melindungi infrastruktur yang menjalankan semua layanan yang ditawarkan di AWS Cloud. Infrastruktur ini terdiri atas perangkat keras, perangkat lunak, jaringan, dan fasilitas yang menjalankan layanan AWS Cloud. Sedangkan, Pelanggan bertanggung jawab atas enkripsi data saat istirahat dan data dalam transit. Pelanggan juga harus memastikan bahwa jaringan dikonfigurasi untuk keamanan dan kredensial keamanan dan login dikelola dengan aman.

AWS bertanggung jawab atas keamanan dari cloud. Jadi, AWS bertanggung jawab atas infrastruktur fisik yang menyediakan sumber daya Anda, termasuk:
- Keamanan fisik pusat data
- Infrastruktur perangkat keras
- Infrastruktur perangkat lunak
- infrasrtuktur jaringan

Pelanggan bertanggung jawab atas apa yang dilaksanakan dengan menggunakan layanan AWS dan untuk aplikasi yang terhubung ke AWS. Jadi,  Pelanggan bertanggung jawab mengelola persyaratan keamanan konten sensitif, termasuk:
- Konten yang pelanggan pilih untuk disimpan di AWS
- Layanan AWS yang digunakan bersama konten
- Di negara mana konten tersebut disimpan Format dan struktur dari konten tersebut, serta apakah konten tersebut disembunyikan, dianonimkan, atau dienkripsi
- Pelanggan yang memiliki akses ke konten tersebut serta bagaimana akses itu diberikan, dikelola, dan ditarik kembali

Jadi, siapa yang bertanggung jawab untuk menjaga keamanan? AWS atau pelanggan? jawabannya ialah semua pihak bertanggung jawab dan saling melengkapi.

## Bagian 2: AWS Identity and Access Management (atau IAM)

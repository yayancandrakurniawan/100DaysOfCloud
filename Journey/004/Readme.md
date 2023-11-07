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

AWS Identity and Access Management (IAM)memungkinkan Anda mengontrol akses ke komputasi, penyimpanan, basis data, dan layanan aplikasi di AWS Cloud. IAM adalah alat yang secara terpusat mengelola akses untuk meluncurkan, mengonfigurasi, mengelola, dan mengakhiri sumber daya di akun AWS Anda. IAM adalah fitur akun AWS yang ditawarkan tanpa biaya tambahan.

**Pengguna IAM** adalah orang atau aplikasi yang ditentukan dalam akun AWS, dan harus membuat panggilan API ke produk AWS. 
Autentikasi adalah konsep keamanan komputer dasar pengguna atau sistem harus terlebih dahulu membuktikan identitas mereka. JIka anda menentukan pengguna IAM. Anda memilih jenis akses yang diizinkan pengguna untuk digunakan. Ada dua jenis autentikasi untuk mendapatkan akses:
- Akses program
  - Autentikasi menggunakan :
      - Access key ID
      - Secret access key
  - Menyediakan akses WS CLI dan AWS SDK
- Akses AWS Management Console
  - Autentikasi menggunakan :
      - ID akun 12 digit atau alias 
      - nama pengguna dan kata sandi IAM
  - Jika otentikasi multifaktor (MFA) diaktifkan untuk pengguna, mereka juga akan dimintai kode autentikasi.

**Grup IAM** adalah pengguna IAM. Anda dapat menggunakan grup IAM umtuk menyederhanakan penentuan dan pengelolaan izin untuk beberapa pengguna. 

Karakteristik penting dari grup IAM:
- Sebuah grup dapat berisi banyak pengguna, dan pengguna dapat menjadi milik beberapa grup.
- Grup tidak dapat ditumpuk. Grup hanya dapat berisi pengguna, dan grup tidak dapat berisi grup lain.
- Tidak ada grup default yang secara otomatis mencakup semua pengguna di akun AWS. Jika Anda ingin memiliki  grup dengan semua pengguna akun di dalamnya, Anda perlu membuat grup dan menambahkan setiap pengguna baru ke dalamnya

**Kebijakan IAM** adalah dokumen yang menetapkan izin untuk menentukan apa yang dapat dilakukan pengguna di akun AWS. 

Terdapat dua jenis kebijakan IAM:
- Kebijakan berbasis identitas
  
  Kebijakan berbasis identitas dapat dikategorikan lebih lanjut sebagai:
  - Kebijakan terkelola –Kebijakan berbasis identitas yang mandiri yang dapat Anda lampirkan pada beberapa pengguna, grup, dan peran dalam akun AWS Anda
  - Kebijakan inline –Kebijakan yang Anda buat dan kelola, dan yang tertanam secara langsung dalam grup atau peran pengguna tunggal
- Kebijakan berbasis sumber daya

  Kebijakan berbasis sumber daya adalah dokumen kebijakan JSON yang Anda lampirkan pada sumber daya, seperti bucket Amazon S3. Kebijakan ini mengatur tindakan apa yang dapat dilakukan pelaku tertentu pada sumber daya tersebut, dan dalam kondisi apa
 
**IAM role** adalah alat untuk memberikan akses sementara ke sumber daya AWS tertentu dalam akun AWS.

## Bagian 3 Mengamankan akun AWS baru

Ada beberapa cara terbaik untuk mengamankan akun AWS. Berikut beberapa cara-caranya:
- Amankan login dengan otentikasi multifaktor (MFA)
- Hapus access key pengguna root akun
- Membuat pengguna IAM individu dan memberikan izin sesuai dengan prinsip hak istimewa paling minim
- Gunakan grup untuk menetapkan izin kepada pengguna IAM
- Mengkonfigurasi kata sandi yang kuat
- Delegasikan penggunaan peran, alih-alih pembagian kredensian
- memantau aktifitas akun menggunakan AWS Cloud Trail

## Bagian 4 

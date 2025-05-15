1. **What is amqp?**
- AMQP (Advanced Message Queuing Protocol) adalah protokol terbuka untuk pertukaran pesan (messaging) antar-aplikasi. Protokol ini menjamin pesan dikirim, diterima, dan diproses dengan andal dalam arsitektur berbasis antrian.
2. **What does it mean? guest:guest@localhost:5672 , what is the first guest, and what
is the second guest, and what is localhost:5672 is for?**
- guest (pertama): username default untuk autentikasi.
- guest (kedua): password yang dipakai bersama username di atas.
- localhost:5672: alamat localhost yang berarti menjalankan di mesin lokal, dan 5672 adalah port standar tempat broker AMQP mendengarkan koneksi.
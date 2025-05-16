1. **What is amqp?**
- AMQP (Advanced Message Queuing Protocol) adalah protokol terbuka untuk pertukaran pesan (messaging) antar-aplikasi. Protokol ini menjamin pesan dikirim, diterima, dan diproses dengan andal dalam arsitektur berbasis antrian.
2. **What does it mean? guest:guest@localhost:5672 , what is the first guest, and what
is the second guest, and what is localhost:5672 is for?**
- guest (pertama): username default untuk autentikasi.
- guest (kedua): password yang dipakai bersama username di atas.
- localhost:5672: alamat localhost yang berarti menjalankan di mesin lokal, dan 5672 adalah port standar tempat broker AMQP mendengarkan koneksi.

3. **Simulation slow subscriber**
![Simulation slow subscriber](img/Simulation_slow_subscriber.jpg)
Total antrean di “Queued messages” (≈20) yang merupakan jumlah pesan yang sudah dikirim tapi belum di-ack oleh subscriber. Karena publisher mengeluarkan 2 pesan/detik sementara subscriber hanya mem-ack 1 pesan/detik, setiap detik muncul 1 pesan baru yang tertunda—setelah sekitar 20 detik, backlog-nya jadi ≈20 pesan.









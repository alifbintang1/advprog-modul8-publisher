# 1. Berapa banyak data yang terkirim?
Program publisher akan mengirimkan 5 data ke broker pesan dalam satu kali eksekusi.

# 2. Apa arti Publisher dan Subscriber mengakses URL yang sama?
URL "amqp://guest:guest@localhost:5672" yang sama dalam program penerbit dan pelanggan berarti bahwa keduanya menggunakan alamat dan kredensial yang sama untuk terhubung ke broker pesan. Dengan kata lain, mereka berkomunikasi dengan broker pesan yang sama di localhost (mesin yang sama), menggunakan kredensial pengguna "guest" dengan kata sandi "guest" untuk otentikasi, dan port 5672. Hal ini memastikan bahwa penerbit dan pelanggan terhubung ke broker yang sama untuk berkomunikasi.

# Running RabbitMQ as message broker.
![Alt text](image/ss1.jpg)
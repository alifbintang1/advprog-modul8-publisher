# 1. Berapa banyak data yang terkirim?
Program publisher akan mengirimkan 5 data ke broker pesan dalam satu kali eksekusi.

# 2. Apa arti Publisher dan Subscriber mengakses URL yang sama?
URL "amqp://guest:guest@localhost:5672" yang sama dalam program penerbit dan pelanggan berarti bahwa keduanya menggunakan alamat dan kredensial yang sama untuk terhubung ke broker pesan. Dengan kata lain, mereka berkomunikasi dengan broker pesan yang sama di localhost (mesin yang sama), menggunakan kredensial pengguna "guest" dengan kata sandi "guest" untuk otentikasi, dan port 5672. Hal ini memastikan bahwa penerbit dan pelanggan terhubung ke broker yang sama untuk berkomunikasi.

# Running RabbitMQ as message broker.
![Alt text](image/ss1.jpg)

# Sending and processing event.
![Alt text](image/ss4.jpg)
![Alt text](image/ss2.jpg)
![Alt text](image/ss3.jpg)
Pada saat message broker atau RabbitMQ berjalan, ketika program Subscriber dan Publisher kita jalankan (cargo run), maka Publisher akan mengirimkan data ke message broker dan Subscriber akan menerima data tersebut. Pada gambar di atas, kita dapat melihat bahwa Publisher mengirimkan data sekali ke message broker dan Subscriber menerimanya.

# Monitoring chart based on publisher.
![Alt text](image/ss5.jpg)
Dari gambar, terlihat bahwa message rates akan meningkat ketika Publisher mengirimkan data ke message broker. Jika message rates tinggi, maka message broker akan menerima banyak data dari Publisher.
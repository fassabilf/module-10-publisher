# Publisher - README

Nama: Faiz Assabil Firdaus  
NPM: 2306224354

---
### a. Berapa data yang dikirim publisher ke message broker dalam satu kali run?
Publisher mengirim 5 data/event (1 event untuk masing-masing user).

### b. URL "amqp://guest:guest@localhost:5672" sama seperti di subscriber, apa artinya?
URL tersebut adalah alamat koneksi ke RabbitMQ. "guest" (depan) = username, "guest" (belakang) = password, "localhost:5672" = alamat host dan port AMQP RabbitMQ. Publisher dan subscriber terhubung ke broker yang sama.

---
## RabbitMQ Management Dashboard

![RabbitMQ Screenshot](./figs/ss1.png)

Gambar di atas menunjukkan RabbitMQ sudah running, dapat diakses melalui web pada port 15672. Username dan password default adalah guest/guest.

## Mengirim dan Memproses Event

Berikut adalah tampilan console saat publisher mengirim pesan dan subscriber menerima pesannya:

![screenshot_publisher](./figs/ss3.png)
![screenshot_subscriber](./figs/ss2.png)
![screenshot_rabbitmq](./figs/ss4.png)

Publisher mengirim 5 event secara berurutan ke broker, dan subscriber menerima serta memprosesnya satu per satu. Hal ini membuktikan event-driven system berjalan dengan baik antara dua aplikasi terpisah melalui message broker (RabbitMQ).

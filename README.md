# Publisher - README

Nama: Faiz Assabil Firdaus  
NPM: 2306224354

---
### a. Berapa data yang dikirim publisher ke message broker dalam satu kali run?
Publisher mengirim 5 data/event (1 event untuk masing-masing user).

### b. URL "amqp://guest:guest@localhost:5672" sama seperti di subscriber, apa artinya?
URL tersebut adalah alamat koneksi ke RabbitMQ. "guest" (depan) = username, "guest" (belakang) = password, "localhost:5672" = alamat host dan port AMQP RabbitMQ. Publisher dan subscriber terhubung ke broker yang sama.

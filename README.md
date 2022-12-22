# Jobsheet-2-Embedded-System
Jobsheet 2 PROTOKOL KOMUNIKASI DAN SENSOR


Percobaan a.  ESP32 Capacitive Touch Sensor

Memiliki bentuk rangkaian sebagai berikut,

<img width="234" alt="Percobaan a" src="https://user-images.githubusercontent.com/121012286/208862372-7071181a-cccc-42e3-b19e-8e206d495b96.png">

Langkah Kerja :

A. ESP32 Capacitive Touch Sensor

1. Hubungkan kabel jumper Male-to-Female pada Pin D4 ESP32.

2. Buka Arduino IDE dan upload script program berikut ke ESP32.

3. Buka serial monitor untuk melihat raw data. Ubah tampilan serial monitor 
menjadi Serial Plotter pada menu Tools > Serial Plotter. 

4. Sentuh ujung kabel jumper dan amati yang terjadi, kemudian dokumentasikan 
hasilnya.

5. Buatlah rangkaian seperti di atas.

6. Buatlah program agar LED menyala ketika sensor disentuh, dan LED akan 
mati ketika sensor tidak disentuh.

7. Buatlah program agar ketika sensor disentuh, LED menyala Blink.

8. Buatlah program agar ketika LED menyala, maka pada Serial Monitor akan 
menampilkan angka yang akan bertambah setiap kali sensor disentuh.

9. Tambahkan 2 LED sehingga pada rangkaian terdapat 3 LED. Buatlah 
program agar ketika sensor disentuh, LED menyala menjadi running LED. 
Nyala running LED tersebut adalah bergerak dari kiri ke kanan, kemudian 
kanan ke kiri secara kontinyu

Hasil Percobaan :


https://user-images.githubusercontent.com/121012286/208862472-7b0ab81e-aff9-4405-a813-54164cb233c2.mp4

Berdasarkan hasl dari percobaan di atas, apabila sensor disentuh maka LED akan menyala blink dan mati apabila sensor tidak tersentuh


Percobaan b. Mengakses Sensor DHT 11 (Single Wire / BUS)

Langkah Kerja:

1. Buatlah rangkaian seperti pada Gambar di bawah ini.

Memiliki bentuk rangkaian sebagai berikut,

<img width="257" alt="percobaan b" src="https://user-images.githubusercontent.com/121012286/208863252-d65c231f-2e11-475b-9624-9696a08a255e.png">

2. Install library sensor DHT 11 melalui Sketch > Include Library > Manage 
Libraries. Ketikkan DHT pada kolom pencarian, pilih library yang akan 
diinstall seperti pada Gambar berikut ini. Kemudian install juga Adafruit 
Unified Sensor menggunakan cara yang sama.

3. Buatlah program seperti pada script di bawah ini untuk mengakses sensor 
DHT11. Kemudian upload program tersebut pada ESP32 dan 
dokumentasikan hasilnya. (sudah terlampir pada file)

4. Buatlah program agar ketika suhu rungan mencapai 30 derajat celcius, maka 
ESP32 akan menyalakan LED Merah dan buzzer secara beep (blink). Apabila 
suhu dibawah 30 derajat, ESP32 akan mematikan buzzer dan menyalakan 
LED berbentuk running LED seperti pada Percobaan A. Kemudian 
dokumentasikan hasilnya

Hasil Percobaan :


https://user-images.githubusercontent.com/121012286/208866097-7069f9b7-b7a6-4d17-8354-81ed52b09c5a.mp4

Berdasarkan hasil percobaan di atas, percobaan ini menggunakan sensor suhu dan cara bekerjanya adalah ketika sensor suhu menangkap suhu
di atas 35 derajat celsius maka lampu led akan menyala berkedip.


Perobaan c.  Mengakses Sensor RFID (SPI Communication)

1. Buatlah rangkaian seperti pada gambar di bawah ini.

Memiliki bentuk rangkaian sebagai berikut,

<img width="395" alt="percobaan c" src="https://user-images.githubusercontent.com/121012286/208867240-6044c814-f5c7-4bbb-b8e8-995a53f30441.png">

2. Install Library MFRC522 dari Library Manager.

3. Dekatkan kartu atau Tag RFID ke RFID Reader. Amati dan analisis cara kerja 
programnya.

4. Buatlah program agar Tag RFID yang terbaca sebelumya dapat digunakan 
untuk hak akses. Apabila Tag RFID didekatkan pada Reader, maka LED 
Hijau akan menyala, servo akan bergerak ke kanan (lalu kembali ke posisi 
semula setelah 3 detik) dan di Serial Monitor akan tertampil pesan “Akses 
Diterima, Silahkan Masuk”. Apabila Tag RFID tidak dikenali, maka LED 
Merah akan menyala, servo tidak bergerak dan di Serial Monitor akan 
tertampil pesan “Akses Ditolak”. Gunakan Tag RFID lain untuk mencoba.

5. Amati yang terjadi, analisis dan dokumentasikan hasilnya.

Hasil Percobaan:


https://user-images.githubusercontent.com/121012286/208868150-36ce5ee0-06b0-47fb-9c99-ed06a8dc09cb.mp4

Berdasarkan percobaan di atas, cara kerja dari percobaan ini adalah dengan menggunakan sensor dan kartu yang akan terdeteksi oleh sensor tersebut,
apabila sensor mendeteksi kartu maka pada serial monitor akan muncul pemberitahuan bahwa Akses diterima.

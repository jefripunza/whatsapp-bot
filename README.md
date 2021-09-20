![banner](icon.svg)

---

[![Custom badge](https://img.shields.io/endpoint?style=for-the-badge&url=https%3A%2F%2Fjefripunza-youtube-channel-badge.vercel.app%2Fapi%2Fsubscriber)](https://www.youtube.com/user/jefripunza/)
[![Custom badge](https://img.shields.io/endpoint?style=for-the-badge&url=https%3A%2F%2Fjefripunza-youtube-channel-badge.vercel.app%2Fapi%2Fviews)](https://www.youtube.com/user/jefripunza/)
[![Custom badge](https://img.shields.io/endpoint?style=for-the-badge&url=https%3A%2F%2Fjefripunza-youtube-channel-badge.vercel.app%2Fapi%2Fcomments)](https://www.youtube.com/user/jefripunza/)
[![Custom badge](https://img.shields.io/endpoint?style=for-the-badge&url=https%3A%2F%2Fjefripunza-youtube-channel-badge.vercel.app%2Fapi%2Fvideos)](https://www.youtube.com/user/jefripunza/videos/)

# Donate

[![Donate](https://img.shields.io/badge/paypal-%2300457C.svg?&style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/jefripunza)

# Sosial Media

[![Custom badge](https://img.shields.io/badge/youtube-%23FF0000.svg?&style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/user/jefripunza/)
[![Custom badge](https://img.shields.io/badge/instagram-%23E4405F.svg?&style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/jefripunza/)
[![Custom badge](https://img.shields.io/badge/facebook-%231877F2.svg?&style=for-the-badge&logo=facebook&logoColor=white)](https://fb.com/jefripunza/)
[![Custom badge](https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/jefripunza/)
[![Custom badge](https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jefri-herdi-triyanto-ba76a8106/)
[![Custom badge](https://img.shields.io/badge/Website-FF7139?style=for-the-badge&logo=Firefox-Browser&logoColor=white)](https://jefriherditriyanto.com/)




# Introduction
[![Custom badge](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Custom badge](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)](https://expressjs.com/)
[![Custom badge](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](https://www.javascript.com/)
[![Custom badge](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://github.com/pedroslopez/whatsapp-web.js/)
[![Custom badge](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/)
[![Custom badge](https://img.shields.io/badge/Google%20Chrome-4285F4?style=for-the-badge&logo=GoogleChrome&logoColor=white)](https://github.com/puppeteer/puppeteer)

WhatsApp kini berkembang pesat seiring dengan waktu yang ada, kebutuhan akan kemampuan WhatsApp perlu ditingkatkan lagi supaya lebih produktif dan efisien. Dengan begitu saya bertekat membuat sebuah WhatsApp BOT untuk anda supaya bisa lebih mudah menjalani kehidupan ini :) ...

---
<br />
<b></b>

# PERSIAPAN

Langkah-langkah persiapan untuk menggunakan project ini untuk user <b>Termux</b> lakukan dari nomor 1 & untuk user <b>Linux Desktop</b> langsung ke nomor 3 :

## 1. install <b>Termux</b>

Download dan install Aplikasi Android Termux dengan cara <a href="https://f-droid.org/repo/com.termux_117.apk" target="_blank" rel="norefferer">klik disini!</a> <br/>

<br />

## 2. install <b>Ubuntu Desktop Environment</b>

### Copy dan Paste di dalam terminal Termux
pada bagian ini membutuhkan waktu estimasi sekitar 20-30 menit tergantung kecepatan internet dan performa perangkat masing-masing.
```bash
wget -qO - https://raw.githubusercontent.com/jefripunza/whatsapp-bot/main/create_ubuntu.sh | bash
```

### Setelah selesai menginstall <b>Ubuntu Desktop Environment</b>, masuk kedalam Environment nya...

```bash
./start-ubuntu.sh
```
<br />

## 3. install <b>All Requirements</b> in Ubuntu

### Copy dan Paste di dalam terminal Termux (Ubuntu)

```bash
wget -qO - https://raw.githubusercontent.com/jefripunza/whatsapp-bot/main/install.sh | bash
```

<br />

---
<br />


# PENGGUNAAN

Didalam penggunaannya <b>"WhatsApp BOT"</b> hal yang paling pertamakali dilakukan adalah <b>Scan Barcode</b> pada Panel.

<br />

## Cara Membuka Panel WhatsApp BOT

### 1. Start Aplikasi didalam Termux (Ubuntu)
#### jika anda berada diluar ubuntu environtment
I. Masuk ke ubuntu environtment
```bash
cd && ./start-ubuntu.sh
```
II. Start Aplikasi
```bash
cd && nodemon
```
#### jika anda berada didalam ubuntu environtment (Linux Desktop)
```bash
cd && nodemon
```

### 2. Lihatlah IP:PORT lokal anda

### 3. Buka IP:PORT di Browser HP (hanya bisa dibuka di HP)

### 4. Login pada Panel
password default :
```bash
12345678
```
bisa anda rubah passwordnya pada file <b>password</b>

<br />

## Cara Scan Barcode (untuk pertama kali/new session)

### 1. Harus menggunakan 2 HP
Hape ke 1 adalah <b>pemilik Whatsapp</b> dan Hape ke 2 adalah bertugas untuk <b>login panel & view barcode</b>

### 2. Tunggu sampai aplikasi mendapatkan session
setelah mendapatkan session maka akan otomatis merubah tampilan ke dalam panel

<br />

## Cara menambah Balasan Chat WhatsApp
1. klik tombol <b>Tambah Balasan</b>
2. isi inputan untuk <b>menerima</b> dan <b>balasan</b>
3. setelah itu klik tombol <b>Tambah</b>

Selebihnya anda bisa merubah data dan menghapusnya. Semua yang tersimpan akan dieksekusi jika <b>menerima</b> pesan yang sesuai dengan data yang ada.

<br />

---
<br />



<br />

# Support the project

Apakah kamu menyukai project ini? Please support saya dengan menekan subscribe di [Youtube Channel](https://www.youtube.com/user/jefripunza/videos/) saya...

<br />

# Donation Please

Butuh ngopi gans, kasih lah untuk biaya pengembangan agar mudah membeli alat dan buat makan <br />
[![Donate](https://img.shields.io/badge/paypal-%2300457C.svg?&style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/jefripunza)

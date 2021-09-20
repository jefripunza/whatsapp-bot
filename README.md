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
[![Custom badge](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://www.whatsapp.com/)
[![Custom badge](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)](https://www.youtube.com/)
[![Custom badge](https://img.shields.io/badge/Google%20Chrome-4285F4?style=for-the-badge&logo=GoogleChrome&logoColor=white)](https://github.com/puppeteer/puppeteer)

WhatsApp kini berkembang pesat seiring dengan waktu yang ada, kebutuhan akan kemampuan WhatsApp perlu ditingkatkan lagi supaya lebih produktif dan efisien. Dengan begitu saya bertekat membuat sebuah WhatsApp BOT untuk anda supaya bisa lebih mudah menjalani kehidupan ini :) ...

---

<br />

# PERSIAPAN

Langkah-langkah untuk menggunakan project ini :

## 1. install <b>Termux</b>

Download dan install Aplikasi Android Termux dengan cara <a href="https://f-droid.org/repo/com.termux_117.apk" target="_blank" rel="norefferer">klik disini!</a> <br/>



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


## 3. install <b>All Requirements</b> in Ubuntu

### Copy dan Paste di dalam terminal Termux

```bash
wget -qO - https://raw.githubusercontent.com/jefripunza/whatsapp-bot/main/install.sh | bash
```


<br />


# PENGGUNAAN

Didalam penggunaannya terdapat sistem CRUD yang di inisialkan sebagai <b>"execute"</b> yang terdiri dari <b>list, clear, add, edit, & delete</b>.

## List data

```javascript
function getData() {
  const data = JSON.parse(
    $.ajax({
      type: "GET",
      url: url + `?password=${password}&execute=list`,
      async: false,
    }).responseText
  );
  if (data.success) {
    return data.data;
  } else {
    return {
      message: "request error!",
    };
  }
}
```

## Clear data

```javascript
sendRequest("clear", {}, (response) => {
    if (response.success) {
        // ok
    } else {
        // error
    }
});
```

## Add data

Struktur data yang akan disimpan SANGAT BERGANTUNG pada object yang di kirim! <br/>
Misal, kita mempunyai object {name: name, message: message} maka struktur yang akan tersimpan di satu data ini mempunyai kolom / key name & message.

```javascript
sendRequest("add", {
        name,
        message,
    }, (response) => {
        if (response.success) {
            // ok
        } else {
            // error
        }
    }
);
```

## Edit data

Diwajibkan menggunakan index select menggunakan key <b>"id"</b> dan value nya dari nilai data <b>"_id"</b> untuk memilih data mana yang akan diubah dan menambahkan object lain selain <b>"id"</b> untuk merubah value nya (multi).

```javascript
sendRequest("edit", {
        id: "value from _id", // index select
        message, // change value from key
    }, (response) => {
        if (response.success) {
            // ok
        } else {
            // error
        }
    }
);
```

## Delete data

Diwajibkan menggunakan index select menggunakan key <b>"id"</b> dan value nya dari nilai data <b>"_id"</b> untuk memilih data mana yang akan dihapus.

```javascript
sendRequest("delete", {
        id: "value from _id", // index select
    }, (response) => {
        if (response.success) {
            // ok
        } else {
            // error
        }
    }
);
```

<br />

# DEVELOPMENT MODE

untuk menjalankan project ini secara development dengan cara (windows) buka file <b>webserver.bat</b> lalu isikan port : 8888

<br />

# Support the project

Apakah kamu menyukai project ini? Please support saya dengan menekan subscribe di [Youtube Channel](https://www.youtube.com/user/jefripunza/videos/) saya...

<br />

# Donation Please

Butuh ngopi gans, kasih lah untuk biaya pengembangan agar mudah membeli alat dan buat makan <br />
[![Donate](https://img.shields.io/badge/paypal-%2300457C.svg?&style=for-the-badge&logo=paypal&logoColor=white)](https://www.paypal.com/paypalme/jefripunza)

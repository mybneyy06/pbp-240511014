# Analisis Platform: Web, Desktop, dan Mobile

**Mata Kuliah:** Pemrograman Berbasis Platform
**Tugas:** Pertemuan 1 – Eksplorasi Platform & Setup Environment
**Nama / NIM:** Naila Fazilatun Nisa / 240511014

## 1. Tabel Analisis Komparatif

| Aspek | Web | Desktop | Mobile |
|---|---|---|---|
| **Bahasa utama** | HTML, CSS, JavaScript/TypeScript (front-end); JavaScript (Node.js), PHP, Python, Java, Go (back-end) | C# (.NET/WPF/WinForms), C++ (Qt), Java (JavaFX/Swing), Python (Tkinter/PyQt), JavaScript (Electron) | Kotlin & Java (Android), Swift (iOS), Dart (Flutter), JavaScript/TypeScript (React Native) |
| **Arsitektur** | Client-server: browser (client) mengirim request HTTP ke server, server membalas dengan HTML/JSON. Umumnya berlapis (presentation – business logic – database), bisa REST API, SPA, atau microservices | Aplikasi *standalone* yang berjalan langsung di OS dan memakai API sistem operasi. Umumnya monolitik/berlapis (UI – logic – data lokal), dapat bersifat offline atau client-server | Aplikasi berjalan di OS mobile dalam *sandbox*, dengan siklus hidup (lifecycle) ketat, dan biasanya terhubung ke backend/API. Pola umum: MVC, MVVM, Clean Architecture |
| **Cara distribusi** | Di-deploy ke server/hosting/cloud lalu diakses lewat URL; tidak perlu instalasi (update langsung oleh developer) | Installer (.exe, .msi, .dmg, .deb), Microsoft Store, Mac App Store, atau portable; pengguna harus mengunduh dan memasang | Toko aplikasi resmi (Google Play Store, Apple App Store), melalui proses review; bisa juga APK langsung (Android) |
| **Keunggulan** | Lintas platform (cukup browser); mudah di-update dan di-maintain terpusat; jangkauan pengguna luas; biaya distribusi rendah | Performa tinggi; akses penuh ke hardware dan file sistem; dapat bekerja offline; cocok untuk aplikasi berat (editor, IDE, CAD) | Portabel dan selalu dibawa pengguna; akses sensor (GPS, kamera, NFC, biometrik); notifikasi push; pengalaman pengguna yang native |
| **Keterbatasan** | Bergantung pada koneksi internet; performa dan akses hardware terbatas oleh browser; isu kompatibilitas antar-browser; risiko keamanan web (XSS, CSRF) | Perlu instalasi dan update manual per perangkat; bergantung pada OS (kecuali memakai framework lintas platform); jangkauan lebih sempit dibanding web | Sumber daya terbatas (baterai, memori, layar kecil); fragmentasi perangkat dan versi OS (Android); proses review toko aplikasi; biaya akun developer |
| **Contoh aplikasi** | Google Docs, Tokopedia (web), Wikipedia, GitHub | Microsoft Word, Visual Studio Code, Adobe Photoshop, VLC Media Player | WhatsApp, Gojek, Instagram, Google Maps |

## 2. Sumber Referensi

1. Mozilla Developer Network. *Learn Web Development*. https://developer.mozilla.org/en-US/docs/Learn_web_development
2. Android Developers. *Platform architecture & App fundamentals*. https://developer.android.com/guide/platform
3. Electron. *Official Documentation – Building cross-platform desktop apps*. https://www.electronjs.org/docs/latest/
4. Microsoft Learn. *Windows app development documentation*. https://learn.microsoft.com/en-us/windows/apps/
5. Node.js. *Introduction to Node.js*. https://nodejs.org/en/learn

## 3. Refleksi

Platform yang paling menarik bagi saya adalah **web**. Alasannya, web memiliki jangkauan paling luas karena aplikasi cukup dibuka lewat browser tanpa instalasi, sehingga hasil karya bisa langsung dicoba oleh siapa pun. Teknologinya juga relatif mudah dimulai, dengan dokumentasi dan komunitas yang sangat besar. Selain itu, kemampuan web kini semakin luas lewat PWA dan framework modern, sehingga satu basis kode dapat menjangkau pengguna desktop maupun mobile.

Tantangan terbesar saat setup environment adalah ukuran file instalasi yang besar, terutama Android Studio beserta SDK dan emulator, yang membutuhkan kuota internet dan ruang penyimpanan banyak. Tantangan lain adalah memastikan semua tools terpasang dengan benar, misalnya konfigurasi PATH untuk Java JDK dan Node.js agar perintah dapat dijalankan di terminal, serta memahami autentikasi GitHub saat melakukan clone dan push.

Rencana saya untuk mengatasinya: mengunduh installer saat koneksi stabil dan memprioritaskan tools yang wajib lebih dulu (Git, Node.js, VS Code, JDK), lalu memasang Android Studio menyusul dan melaporkannya sesuai ketentuan tugas. Saya akan memeriksa setiap instalasi lewat perintah versi di terminal, membaca dokumentasi resmi ketika muncul galat, dan memastikan ruang penyimpanan cukup sebelum memasang. Untuk GitHub, saya akan memakai Personal Access Token atau SSH key agar proses push berjalan lancar.

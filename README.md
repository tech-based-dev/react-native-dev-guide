![alt text][tllogo]

Daftar Isi
=====================
* [Guide Pengembangan Aplikasi React Native](#guide-pengembangan-aplikasi-react-native)
* [Penjelasan Singkat React Native](#penjelasan-singkat-react-native)
* [Setup Environment](#setup-environment)
    * [Hardware](#hardware)
    * [Software](#software)
    * [Network](#network)
* [Hands-on Overview](#hands-on-overview)

# Guide Pengembangan Aplikasi React Native
Dokumen ini merupakan guide untuk menyiapkan keperluan dalam mengembangkan aplikasi react native di Windows, MacOS, dan Linux. Perlu diketahui bahwa mengembangkan aplikasi mobile dengan menggunakan React Native dapat dilakukan dengan dua cara, yaitu menggunakan Expo atau React Native CLI. Pada dokumen ini, difokuskan untuk mengembangkan aplikasi React Native dengan menggunakan React Native CLI (Command Line Interface). Ada yang tahu beda antara keduanya?

# Penjelasan Singkat React Native
https://facebook.github.io/react-native/docs/getting-started

# Setup Environment
Bagian ini menjelaskan apa saja yang harus disiapkan untuk membuat sebuah aplikasi React Native, dari segi hardware, software, dan network.

## Hardware
Pastikan kamu memiliki hardware dengan spesifikasi minimum sebagai berikut:

* Laptop (RAM >= 2GB, Storage >= 4GB)
* Smartphone Android yang sudah memiliki [Developer Options](https://www.digitaltrends.com/mobile/how-to-get-developer-options-on-android/)
* Kabel penghubung smartphone ke komputer

## Software
Setup environment sangat bergantung pada sistem operasi yang digunakan pada masing-masing komputer. Berikut ini dijelaskan environment untuk masing-masing sistem operasi.

### Android
Android Lolipop (atau lebih baru) dengan Developer Options

### Windows

### MacOS

#### Instalasi Editor Teks
Editor teks merupakan alat utama dalam membuat sebuah aplikasi, baik mobile, web, maupun desktop. Setiap orang memiliki preferensinya masing-masing dalam memilih editor teks ini. Berikut ini pilihan yang bisa dieksplorasi apabila kamu tertarik untuk eksplorasi lebih jauh. Editor teks yang direkomendasikan oleh kami dicetak lebih tebal dibanding yang lainnya.

Basic:
* [**Sublime Text**](https://www.sublimetext.com)
* [Visual Studio Code](https://code.visualstudio.com)

Intermediate:
* [WebStorm](https://www.jetbrains.com/webstorm/)

Advance:
* [Vim](https://www.vim.org)
* [Emacs](https://www.gnu.org/software/emacs/)

#### Persiapan Terminal
Terminal adalah sebuah aplikasi yang dapat digunakan untuk berinteraksi dengan berbagai program tanpa harus mengakses grafisnya (GUI). Terminal ini akan digunakan untuk memulai proyek, menjalankan, hingga memonitor hasilnya. MacOS sebenarnya telah memiliki aplikasi terminal default out-of-the-box bernama "Terminal". Aplikasi ini bisa diakses dengan membuka direktori Application, kemudian cari aplikasi bernama "Terminal". Alternatif lainnya adalah dengan menggunakan aplikasi lain yang memiliki fungsi lebih banyak bernama [iTerm2](https://www.iterm2.com). 

#### Instalasi Homebrew (via terminal)
Homebrew adalah sebuah aplikasi yang berjalan di atas terminal dan digunakan untuk mengelola aplikasi, biasanya aplikasi-aplikasi yang diperlukan dalam pengembangan software. Untuk lebih jelas mengenai homebrew, informasinya dapat dilihat di https://brew.sh. Kamu bisa mengikuti langkah-per-langkah yang ada di website tersebut dan mengeksplorasi kemungkinan-kemnungkinannya. Sebagai gambaran sederhana, berikut ini cuplikan yang diperlukan dan relevan dalam dokumen ini.

Ketikkan perintah ini melalui terminal untuk menginstall homebrew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Ketika sudah selesai, pastikan homebrew terinstall dengan mengetik perintah berikut ini:
```
brew -v
```

Keluaran dari perintah itu mirip seperti keluaran di bawah ini, yang artinya brew sudah berhasil diinstal dengan baik:
```
⇒  brew -v
Homebrew 2.0.0
Homebrew/homebrew-core (git revision 64b29; last commit 2019-02-06)
Homebrew/homebrew-cask (git revision 3dd068; last commit 2019-02-06)
```

#### Instalasi Node JS & Node Package Manager (NPM)
Aplikasi berikutnya yang harus diinstall adalah Node JS. Aplikasi ini dapat diinstall melalui Homebrew yang telah diinstall pada bagian sebelumnya. Instalasi dapat dilakukan dengan mengetikkan perintah berikut ini:
```
brew install node
```

Pastikan node JS sudah terpasang dengan mencari tahu versi yang terpasang
```
node -v
```

Begitu pula pastikan NPM sudah terpasang dengan mencari tahu versinya.
```
npm -v
```

#### Instalasi Watchman
Berikutnya, install watchman yang dibutuhkan untuk memonitor aplikasi react native secara real-time.
```
brew install watchman
```

#### Instalasi React Native CLI
Bagian paling penting dalam instalasi ini adalah pemasangan React Native, yang dapat diinstall dengan mengetikkan perintah berikut ini:
```
npm install -g react-native-cli
```

Apabila react native sudah terpasang, cek versi yang terinstall dengan mengetikkan perintah berikut ini:
```
⇒  react-native -v
react-native-cli: 1.3.0
react-native: 0.57.8
```

### Linux

## Network
Pastikan kamu terhubung ke Internet

# Hands-on Overview

[tllogo]: https://i.imgur.com/hLjs5wq.png "techlab Logo"

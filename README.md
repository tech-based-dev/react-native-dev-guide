![alt text][tllogo]

Daftar Isi
=====================
* [Guide Pengembangan Aplikasi React Native](#guide-pengembangan-aplikasi-react-native)
* [Penjelasan Singkat React Native](#penjelasan-singkat-react-native)
* [Setup Environment](#setup-environment)
    * [Network](#network)
    * [Hardware](#hardware)
    * [Software](#software)
* [Hands-on Overview](#hands-on-overview)

# Guide Pengembangan Aplikasi React Native
Dokumen ini merupakan guide untuk menyiapkan keperluan dalam mengembangkan aplikasi react native di laptop Windows, MacOS, dan Linux. Perlu diketahui bahwa mengembangkan aplikasi mobile dengan menggunakan React Native dapat dilakukan dengan dua cara, yaitu menggunakan Expo atau React Native CLI. Pada dokumen ini, difokuskan untuk mengembangkan aplikasi React Native dengan menggunakan Expo. Ada yang tahu beda antara keduanya?

# Penjelasan Singkat React Native
https://facebook.github.io/react-native/docs/getting-started

# Setup Environment
Bagian ini menjelaskan apa saja yang harus disiapkan untuk membuat sebuah aplikasi React Native, dari segi hardware, software, dan network.

## Network
Pastikan kamu terhubung ke Internet. Kamu pasti sudah tahu caranya.

## Hardware
Pastikan kamu menyiapkan hardware dengan spesifikasi minimum sebagai berikut:

* Laptop (RAM >= 2GB, Storage >= 4GB)
* Smartphone Android atau iPhone

## Software
Sebelum bisa memulai membuat aplikasi, kita perlu menyiapkan program-program pendukungnya, program-program ini biasa disebut dengan environment. Ada beberapa bagian dari setup environment ini yang sangat bergantung pada sistem operasi yang digunakan pada masing-masing komputer, misalnya instalasi NPM di macOS, Linux, dan Windows akan memiliki perbedaan cara. Berikut ini akan dijelaskan cara instalasi environment untuk masing-masing program, dan apabila ada program yang memerlukan perlakuan instalasi khusus pada sistem operasi tertentu, maka akan dijelaskan pada setiap bagiannya. Silakan pilih cara instalasi sesuai dengan sistem operasi yang dimiliki.

### Instalasi Expo
Untuk mengembangkan aplikasi React Native dengan menggunakan Expo di Android atau iOS, tentunya kamu harus memasang aplikasi bernama [Expo](https://expo.io) dari Google Play Store untuk Android, atau App Store untuk iOS. Pastikan kamu pasang aplikasi ini di smartphone kamu.

### Instalasi Editor Teks
Editor teks merupakan alat utama dalam membuat sebuah aplikasi, baik mobile, web, maupun desktop. Setiap orang memiliki preferensinya masing-masing dalam memilih editor teks ini. Berikut ini pilihan yang bisa dieksplorasi apabila kamu tertarik untuk eksplorasi lebih jauh. Editor teks yang direkomendasikan oleh kami dicetak lebih tebal dibanding yang lainnya.

Basic:
* [**Sublime Text**](https://www.sublimetext.com)
* [Visual Studio Code](https://code.visualstudio.com)

Intermediate:
* [WebStorm](https://www.jetbrains.com/webstorm/)

Advance:
* [Vim](https://www.vim.org)
* [Emacs](https://www.gnu.org/software/emacs/)

### Persiapan Terminal
Terminal adalah sebuah aplikasi yang dapat digunakan untuk berinteraksi dengan berbagai program tanpa harus mengakses grafisnya (GUI). Terminal ini akan digunakan untuk memulai proyek, menjalankan, hingga memonitor hasilnya. 

#### MacOS
MacOS sebenarnya telah memiliki aplikasi terminal default out-of-the-box bernama "Terminal". Aplikasi ini bisa diakses dengan membuka direktori Application, kemudian cari aplikasi bernama "Terminal". Alternatif lainnya adalah dengan menggunakan aplikasi lain yang memiliki fungsi lebih banyak bernama [iTerm2](https://www.iterm2.com). 

![alt text][iterm2]

#### Linux
Lnux telah memiliki aplikasi terminal default out-of-the-box bernama "Terminal". Aplikasi ini bisa ditemukan dengan mencari aplikasi dengan keyword "terminal".

![alt text][ubuntuterminal]

#### Windows
Terminal pada windows dikenal dengan nama command prompt atau cmd. Command prompt bisa diakses dengan beberapa cara. Cara yang pertama adalah dengan mencari aplikasi dengan keyword "command prompt". Cara yang kedua adalah dengan menekan tombl window + r yang memunculkan dialog "run", kemudian tuliskan "cmd" (tanpa tanda kutip), kemudian tekan enter.

![alt text][cmd]

### Instalasi Node JS & Node Package Manager (NPM)
![alt text](https://dev.acquia.com/sites/default/files/styles/blog_node_image/public/blog/nodejs-new-pantone-black2.png "Node JS")

#### MacOS

##### Instalasi Homebrew (via terminal)
Homebrew adalah sebuah aplikasi yang berjalan di atas terminal dan digunakan untuk mengelola aplikasi, biasanya aplikasi-aplikasi yang diperlukan dalam pengembangan software. Untuk lebih jelas mengenai homebrew, informasinya dapat dilihat di https://brew.sh. Kamu bisa mengikuti langkah-per-langkah yang ada di website tersebut dan mengeksplorasi kemungkinan-kemnungkinannya. Sebagai gambaran sederhana, berikut ini cuplikan yang diperlukan dan relevan dalam dokumen ini. Buka terminal yang sudah disiapkan, kemuduan ketikkan perintah ini melalui terminal untuk menginstall homebrew.
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

##### Instalasi Node JS dan NPM (Node Package Manager)
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

##### Instalasi Expo CLI
Expo adalah sebuah aplikasi yang terdapat di dalam komputer dan smartphone kamu yang mempermudah pembuatan aplikasi menggunakan React Native. Expo CLI adalah aplikasi yang dipasang di dalam komputer kamu, dapat dilakukan dengan cara mengetikkan perintah berikut:
```
npm install -g expo-cli
```

#### Linux (debian-based)
Langkah-langkah pada bagian ini menganggap kamu menggunakan APT yang terdapat pada debian-based atau beberapa distro lainnya. Apabila kamu menggunakan package manager selain APT, silakan kontak fasilitator terdekat.

##### Instalasi Node JS dan NPM (Node Package Manager)
Aplikasi berikutnya yang harus diinstall adalah Node JS. Aplikasi ini dapat diinstall melalui APT yang telah ada secara out-of-the-box pada bagian sebelumnya. Instalasi dapat dilakukan dengan mengetikkan perintah berikut ini satu per satu:

Instalasi curl
```
sudo apt install curl
```

Menambahkan PPA
```
curl -sL https://deb.nodesource.com/setup_8.x | sudo bash -
```

Instalasi NodeJS
```
sudo apt install nodejs
```

Pastikan node JS sudah terpasang dengan mencari tahu versi yang terpasang
```
node -v
```

Begitu pula pastikan NPM sudah terpasang dengan mencari tahu versinya.
```
npm -v
```

##### Instalasi Expo CLI
Expo adalah sebuah aplikasi yang terdapat di dalam komputer dan smartphone kamu yang mempermudah pembuatan aplikasi menggunakan React Native. Expo CLI adalah aplikasi yang dipasang di dalam komputer kamu, dapat dilakukan dengan cara mengetikkan perintah berikut:
```
npm install -g expo-cli
```
#### Windows
##### Instalasi Node JS dan NPM (Node Package Manager)
Pemasangan Node JS di Windows dapat dilakukan dengan mengunduh installer di [https://nodejs.org/en/download/](https://nodejs.org/en/download/), kemudian memilih installer Node JS dengan tipe LTS. Setelah selesai mengunduh, silakan eksekusi file yang baru saja diunduh dan ikuti instruksi selanjutnya.

Pastikan node JS sudah terpasang dengan mencari tahu versi yang terpasang dengan mengetikkan perintah ini di command prompt (tutup terlebih dahulu comand prompt yang sebelumnya dibuka, kemudian buka kembali yang baru).
```
node -v
```

Begitu pula pastikan NPM sudah terpasang dengan mencari tahu versinya.
```
npm -v
```

##### Instalasi Expo CLI
Expo adalah sebuah aplikasi yang terdapat di dalam komputer dan smartphone kamu yang mempermudah pembuatan aplikasi menggunakan React Native. Expo CLI adalah aplikasi yang dipasang di dalam komputer kamu, dapat dilakukan dengan cara mengetikkan perintah berikut:
```
npm install -g expo-cli
```

[tllogo]: https://i.imgur.com/hLjs5wq.png "techlab Logo"
[iterm2]: https://i.imgur.com/75NUPpT.png "iterm2"
[cmd]: https://upload.wikimedia.org/wikipedia/commons/b/b3/Command_Prompt_on_Windows_10_RTM.png
[ubuntuterminal]: https://www.howtogeek.com/wp-content/uploads/2013/03/xlinux-terminal-on-ubuntu.png.pagespeed.gp+jp+jw+pj+ws+js+rj+rp+rw+ri+cp+md.ic.-XaWFngjEl.png

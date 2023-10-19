# GOLANG MODULES

## Perkenalan

- Saat kita membuat aplikasi, biasanya kita akan menggunakan library atau
  depedency dari project lain.
- Sebelum ada Go Modules, management untuk depedency sangat sulit dilakukan di
  Go-Lang
- Biasanya kita akan meng-copy semua source code library atau depedency lain ke
  project kita, hal ini membuat project kita menjadi bengkak karena penuh dengan
  library orang lain.
- Atau biasanya library orang lain akan kita save di GOPATH directory, namun hal
  ini akan sulit jika ternyata beberapa aplikasi butuh library yang sama dengan
  versi yang berbeda.

## Go-Modules

- Go-Modules mulai dikenalkan di Go-Lang 1.11 dan 1.12.
- Dengan Go-Modules, kita bisa membuat project dengan mudah dan depedency
  management yang sangat mudah.

## Membuat Module

- Untuk membuat module baru, kita bisa menggunakan perintah: go mod init
  nama-module
- Go-Lang akan secara otomatis membuat file go.mod yang berisikan informasi nama
  module dan juga versi Go-Lang yang kita gunakan

## Rilis Module

- Go-Lang terintegrasi baik dengan Git
- Untuk merilis module, kita hanya perlu membuat Tag di Git

## Upgrade Module

- Untuk melakukan upgrade module, kita hanya cukup membuat tag baru di Git

## Upgrade Depedency

- Untuk upgrade depedency ke versi terbaru, kita bisa mengubah isi go.mod, lalu
  mengubah tag nya menjadi tag terbaru
- Untuk mendownload versi terbaru, gunakan perintah: go get

## Major Upgrade

- Major upgrade biasanya terjadi dikarenakan ada perubahan pada isi kode program
  kita, sehingga membuat tidak backward compatible
- Sebaiknya hal ini sebisa mungkin dihindari
- Namun jika tidak bisa dihindari, strategy terbaik adalah merubah nama module


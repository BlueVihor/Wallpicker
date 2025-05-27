# Maintainer Sukhov Daniil <tech@accountt.ru> https://github.com/BlueVihor
pkgname=wallpicker
pkgver=1.0
pkgrel=1
pkgdesk="Wallpaper picker written in bash"
arch=('any')
makedepends=('git'
  'feh'
  'rofi')

prepare() {=
  git clone https://github.com/BlueVihor/Wallpicker.git
  cd Wallpicker
}

package() {
  cd Wallpicker
  sudo cp wallpicker "/usr/bin/"
  sudo chmod 777 "/usr/bin/wallpicker"
}

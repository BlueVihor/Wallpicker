pkgname=wallpicker
pkgver=1.0
pkgrel=1
pkgdesk="Wallpaper picker written in bash"
arch=('any')
makedepends=('git'
  'feh'
  'rofi')

prepare() {
  cd "$srcdir/$pkgname"
}

package() {
  cd "$srcdir/$pkgname"
  cp wallpicker "/usr/bin/"
  chmod 777 "/usr/bin/wallpicker"
}

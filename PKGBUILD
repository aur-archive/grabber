# Archtrack maintainer: Evan Teitelman <teitelmanevan at gmail dot com>
# Contributor: Francesco Piccinno <stack.box@gmail.com>

pkgname=grabber
pkgver=0.1
pkgrel=1
pkgdesc="Grabber is a web application scanner. Basically it detects some kind of vulnerabilities  in your website."
arch=('any')
url="http://rgaucher.info/beta/grabber/"
license=('BSD')
depends=('python')
source=(http://rgaucher.info/beta/$pkgname/Grabber.zip)
md5sums=('29c34fabf5658d2246b03b1b790eedbf')

groups=(archtrack archtrack-web-applications)

build() {
  cd "$srcdir/Grabber"
  chmod -x *
  rm setup.py
  chmod +x grabber.py

  mkdir -p $pkgdir/usr/share/$pkgname
  cp -r * $pkgdir/usr/share/$pkgname/
}

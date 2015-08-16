# Contributor: Lex Black <autumn-wind at web dot de>
# Contributor: Termac <terror.macbeth.I@gmail.com>
# Contributor: Alexander Surma <surma (a) drebesium (.) org>

pkgname=kuechenstation
pkgver=0.4
pkgrel=2
pkgdesc="A leightweight xmms2 console client written in python"
url="http://kuechenstation.sourceforge.net/"
license=('GPL')
arch=('i686' 'x86_64')
makedepends=('python2')
depends=('python2' 'figlet' 'xmms2>=0.6DrMattDestruction-9')
optdepends=('python2-feedparser: podcast support')
source=(http://downloads.sourceforge.net/kuechenstation/${pkgname}_${pkgver}.tar.gz)
md5sums=('a6e47f4ad2be24faadf416e1efa0b4a4')

build() {
   cd $srcdir/$pkgname-$pkgver
   python2 setup.py build
}

package() {
   cd $srcdir/$pkgname-$pkgver
   python2 setup.py install --root=${pkgdir}
}

# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-purchase-invoice-line-standalone
_pkgname=trytond_purchase_invoice_line_standalone
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The purchase_invoice_line_standalone module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-account-invoice-line-standalone>=3.4' 'trytond-purchase>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("894133011b06bc2cc64a3ad270a42817")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}
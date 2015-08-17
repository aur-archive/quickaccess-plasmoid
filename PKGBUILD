# Maintainer: Carl Mueller  arch at carlm e4ward com

pkgname=quickaccess-plasmoid
pkgver=0.8.2
pkgrel=2
pkgdesc='Kdeplasma widget for quick access to folders.'
arch=('i686' 'x86_64')
url='http://kde-look.org/content/show.php/?content=134442'
license=('GPL')
depends=('kdebase-workspace' 'kdebase-plasma')
makedepends=('cmake' 'automoc4')
conflicts=(kde-extragear-plasmoids)
source=(http://kde-look.org/CONTENT/content-files/134442-plasma-widget-quickaccess-$pkgver-$pkgrel.zip)
md5sums=('4879aa3af6d7db8e06dd8ed0ad994a51')
build() {
    cd $srcdir/plasma-widget-quickaccess-$pkgver-$pkgrel/build
    cmake ../ -DCMAKE_INSTALL_PREFIX=`kde4-config --prefix`
    make VERBOSE=1
    make DESTDIR=$pkgdir install
}

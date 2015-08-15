# Contributor: Tibor Bamhor <tiborb95 at gmail.com>

pkgname=cphix
pkgver=1.7.4
pkgrel=1
pkgdesc="Batch processing of photos - auto-enhancement of saturation, sharpness and brightness distribution. Command line tool."
url="http://code.google.com/p/cphix/"
license="GPL-3"
arch=('i686' 'x86_64')
depends=(cimg)
source=(http://cphix.googlecode.com/files/cphix-$pkgver.tgz)



build() {
	#export LDFLAGS="$LDFLAGS -lm"
	
	cd ${srcdir}/cphix
	chmod +x configure.sh
	./configure.sh
	make
}


package() {
	#copying file into pkgdir to be packed
	mkdir -p $pkgdir/usr/bin/

	install -m 755 ${srcdir}/cphix/cphix2.bin $pkgdir/usr/bin/ 
	
}

sha1sums=('94494df7faafe473aa9d7cf4943e3d7cbf0e74f6') 



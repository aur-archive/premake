# Contributor: Anders Bergh <anders1@gmail.com>
# Contributor: Mildred <silkensedai@online.fr>
# Maintainer: Daniel J Griffiths <griffithsdj@archlinux.us>

pkgname=premake
pkgver=3.7
pkgrel=1
pkgdesc="A build configuration tool. Describe your build using Lua and generate \
the project files for your specific toolset."
arch=('i686' 'x86_64')
url="http://premake.sourceforge.net"
license=('GPL')
makedepends=()
source=("http://downloads.sourceforge.net/sourceforge/premake/premake-src-${pkgver}.zip")
md5sums=('8d30dc5bbc52aad81abb1509c1dd7d8f')

build() {
	cd ${srcdir}/Premake-${pkgver}
	make || return 1
}

package() {
	cd ${srcdir}/Premake-${pkgver}
	install -Dm755 bin/premake ${pkgdir}/usr/bin/premake
}

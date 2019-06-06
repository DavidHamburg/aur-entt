# Maintainer: David Nerjes <david.hamburg@googlemail.com>
pkgname=entt
pkgver=3.0.0
pkgrel=1
epoch=
pkgdesc="Gaming meets modern C++ - a fast and reliable entity-component system and much more"
arch=('any')
url="https://github.com/skypjack/entt"
license=('MIT')
groups=()
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(https://github.com/skypjack/$pkgname/archive/v$pkgver.tar.gz
        FindEntt.cmake)
sha256sums=('f8928314a18f1fabda5398efdef7a001d09de43c2ffda90c1b77e56f5d41574b'
            '7e09af7280371470d484c5db4c947801d29b82e6a53aba944fe7d883f6e0b02f')
noextract=()
validpgpkeys=()

package() {
	install -D -m644 "$srcdir/FindEntt.cmake" "${pkgdir}/usr/share/cmake-3.14/Modules/FindEntt.cmake"
	cd "$pkgname-$pkgver"
	install -D -m644 "LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
    mkdir -p "${pkgdir}/usr/lib/include/${pkgname}" 
    cp -r src/entt "${pkgdir}/usr/lib/include/${pkgname}"

}

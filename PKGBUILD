# Maintainer: David Nerjes <david.hamburg@googlemail.com>
pkgname=entt
pkgver=2.7.2
pkgrel=2
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
sha256sums=('26f67fff543ca8c5bb2ee51833e750a4ea59738cdf28779e4e2c90eb0b6f2a5e'
            '7e09af7280371470d484c5db4c947801d29b82e6a53aba944fe7d883f6e0b02f')
noextract=()
validpgpkeys=()

package() {
	install -D -m644 "$srcdir/FindEntt.cmake" "${pkgdir}/usr/share/cmake-3.12/Modules/FindEntt.cmake"
	cd "$pkgname-$pkgver"
	install -D -m644 "LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
    mkdir -p "${pkgdir}/usr/lib/include/${pkgname}" 
    cp -r src/entt "${pkgdir}/usr/lib/include/${pkgname}"

}

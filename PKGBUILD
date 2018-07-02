# Maintainer: David Nerjes <david.hamburg@googlemail.com>
pkgname=entt
pkgver=2.7.1
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
source=("https://github.com/skypjack/$pkgname/archive/v$pkgver.tar.gz")
sha256sums=('50a0387889aa3a28ba24424a2be71d60884aa46534cc0742883c8e7729ed68bc')
noextract=()
md5sums=()
validpgpkeys=()

package() {
	install -D -m644 "../FindEntt.cmake" "${pkgdir}/usr/share/cmake-3.11/Modules/FindEntt.cmake"
	cd "$pkgname-$pkgver"
	install -D -m644 "LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
    mkdir -p "${pkgdir}/usr/lib/include/${pkgname}" 
    cp -r src/entt "${pkgdir}/usr/lib/include/${pkgname}"

}

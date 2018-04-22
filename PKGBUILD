# Maintainer: David Nerjes <david.hamburg@googlemail.com>
pkgname=entt
pkgver=2.5.0
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
sha256sums=('6246501c6589eba9832538c47a23a239eaa1066c77471cae7d79e741141ade82')
noextract=()
md5sums=()
validpgpkeys=()

package() {
	install -D -m644 "../FindEntt.cmake" "${pkgdir}/usr/share/cmake-3.10/Modules/FindEntt.cmake"
	cd "$pkgname-$pkgver"
	install -D -m644 "LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
    mkdir -p "${pkgdir}/usr/lib/include/${pkgname}" 
    cp -r src/entt "${pkgdir}/usr/lib/include/${pkgname}"

}

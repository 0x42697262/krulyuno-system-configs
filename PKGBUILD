# Maintainer: KrulYuno <Discord: Lost Felt#8517>
pkgname=krulyuno-system-configs
pkgver=1.0.0
pkgrel=1
pkgdesc="My personal system configs when installing arch for my laptop."
arch=('any')
url=""
license=('GPL3')
depends=()
makedepends=()
backup=()
source=("$pkgname-$pkgver.tar.gz"
        "$pkgname-$pkgver.patch")
sha256sums=()

prepare() {
	cd "$pkgname-$pkgver"
	patch -p1 -i "$srcdir/$pkgname-$pkgver.patch"
}

package() {
	cd "$pkgname-$pkgver"
	make DESTDIR="$pkgdir/" install
}

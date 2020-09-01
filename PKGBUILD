# Maintainer: Me lmao
pkgname="dmenu"
pkgver=1
pkgrel=1
pkgdesc="dynamic menu for X"
arch=('x86_64')
url='git.suckless.org/dmenu'
license=('MIT')
depends=('libxft-bgra' 'sh' 'libxinerama' 'freetype2')
makedepends=('git')
source=('dmenu::git://github.com/DragonGhost7/dmenu.git')
md5sums=('SKIP')

pkgver() {
cd "$pkgname"
printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

build() {
	cd "$pkgname"
	make
}

package() {
	cd "$pkgname"
	install -Dm755 ./dmenu "$pkgdir/usr/local/bin/dmenu"
	install -Dm644 ./dmenu.1 "$pkgdir/usr/local/man/man1/dmenu.1"
}

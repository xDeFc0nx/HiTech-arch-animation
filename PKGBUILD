# Hi-Tech-arch-animation PKGBUILD

pkgname=hitech-arch-animation
pkgver=1.0
pkgrel=1
pkgdesc="Hi-Tech Arch Linux Plymouth Theme"
arch=('any')
url="https://github.com/xDeFc0nx/HiTech-arch-animation"
license=('MIT')
depends=('plymouth')

pkgver() {
	cd "$srcdir/$pkgname-main"
	git describe --long --tags | sed 's/\([^-]*-g\)/r\1/;s/-/./g'
}

source=("git+${url}.git#commit=HEAD")

package() {
	cd "$srcdir/$pkgname-main"
	cp -r "$pkgname-main/"* "$pkgdir/usr/share/plymouth/themes/$pkgname/"
}

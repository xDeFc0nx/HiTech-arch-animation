# Hi-Tech-arch-animation PKGBUILD

pkgname=hitech-arch-animation
pkgver=1.0
pkgrel=1
pkgdesc="Hi-Tech Arch Linux Plymouth Theme"
arch=('any')
url="https://github.com/xDeFc0nx/Hi-Tech-arch-animation"
license=('MIT')
depends=('plymouth')

source=("$url/archive/main.tar.gz")

build() {
	cd "$srcdir/$pkgname-main"
}

package() {
	cd "$srcdir/$pkgname-main"
	install -Dm644 arch.plymouth "$pkgdir/usr/share/plymouth/themes/$pkgname/arch.plymouth"
	install -Dm644 animated-boot.script "$pkgdir/usr/share/plymouth/themes/$pkgname/animated-boot.script"
	install -Dm644 box.png "$pkgdir/usr/share/plymouth/themes/$pkgname/box.png"

}

# Maintainer: echo -n 'bWF0dEBnZXRjcnlzdC5hbA==' | base64 --decode

pkgname=crystal-grub-theme
pkgver=1.0.1
pkgrel=1
pkgdesc="GRUB Theme for Crystal Linux"
arch=('any')
url="https://github.com/crystal-linux/grub-theme"
depends=('grub')
source=("git+$url")

sha256sums=("SKIP")

package() {
    cd ${srcdir}/grub-theme
    mkdir -p ${pkgdir}/usr/share/grub/themes
    cp -rv crystal ${pkgdir}/usr/share/grub/themes/.
}

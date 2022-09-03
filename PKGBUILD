# Maintainer: echo -n 'bWF0dEBnZXRjcnlzdC5hbA==' | base64 --decode

_name=grub-theme

pkgname="crystal-$_name"
pkgver=1.0.1
pkgrel=1
pkgdesc="GRUB Theme for Crystal Linux"
arch=('any')
url="https://github.com/crystal-linux/$_name"
depends=('grub')
source=("git+$url")

sha256sums=("SKIP")

package() {
    cd ${srcdir}/${_name}
    mkdir -p ${pkgdir}/usr/share/grub/themes
    cp -rv crystal ${pkgdir}/usr/share/grub/themes/.
}

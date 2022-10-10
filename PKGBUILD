# Maintainer:  echo -n 'TWF0dCBDLiA8bWF0dEBnZXRjcnlzdC5hbD4='     | base64 -d
# Contributor: echo -n 'TWljaGFsIFMuIDxtaWNoYWxAZ2V0Y3J5c3QuYWw+' | base64 -d
# Contributor: echo -n 'Um9iaW4gQy4gPHJjYW5kYXVAZ2V0Y3J5c3QuYWw+' | base64 -d


pkgname=crystal-grub-theme
_pkgname=grub-theme
pkgver=1.0.1
pkgrel=2
pkgdesc='GRUB Theme for Crystal Linux'
arch=('any')
url="https://github.com/crystal-linux/${_pkgname}"
license=('MIT')
depends=('grub')
install="${pkgname}.install"
source=("${pkgname}-${pkgver}::${url}/archive/v${pkgver}.tar.gz")
sha256sums=('09d892520164598b5a866c7c82c9c1b55dfd7563a331e2bb01191a0d88d4683c')

package() {
    cd "${srcdir}/${_pkgname}-${pkgver}"        
    install -d "${pkgdir}/usr/share/grub/themes"
    cp -R crystal "${pkgdir}/usr/share/grub/themes/"
    install -Dm 644 "LICENSE" "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
    install -Dm 644 "README.md" "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}

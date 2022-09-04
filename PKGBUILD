# Maintainer:  echo -n 'TWF0dCBDLiA8bWF0dEBnZXRjcnlzdC5hbD4='     | base64 -d
# Contributor: echo -n 'TWljaGFsIFMuIDxtaWNoYWxAZ2V0Y3J5c3QuYWw+' | base64 -d

_name=grub-theme

pkgname="crystal-$_name"
pkgver=1.0.1
pkgrel=1
pkgdesc='GRUB Theme for Crystal Linux'
arch=('any')
license=('MIT')
url="https://github.com/crystal-linux/$_name"
depends=('grub')
makedepends=('git')
source=("git+$url")
sha256sums=('SKIP')

package() {
    cd "$srcdir/$_name"    
    install -Dm 0755 crystal "$pkgdir/usr/share/grub/themes/."
}

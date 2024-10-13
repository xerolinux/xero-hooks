# Maintainer: DarkXero <info@techxero.com>

pkgname=xero-hooks
pkgdesc="Fixes, additions and enhancements to grub and os-prober."
pkgver=1.0.2
pkgrel=1
arch=('any')
license=('GPL')
depends=(grub lsb-release)
optdepends=(os-prober)

url=https://github.com/xerolinux/$pkgname
_url="https://raw.githubusercontent.com/xerolinux/$pkgname/main"

source=(
  $_url/mkinitcpio-gpu.hook
)

package() {
  cd $srcdir

  install -d $pkgdir/usr/share/libalpm/hooks
  install -Dm644 mkinitcpio-gpu.hook $pkgdir/usr/share/libalpm/hooks/mkinitcpio-gpu.hook
}

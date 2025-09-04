# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-swaync-config
pkgver=1.0
pkgrel=1
pkgdesc="Swaync configuration for StratOS"
arch=('any')
license=('GPL3')
depends=(
    'swaync'
)
source=()
install=stratos-swaync-config.install

prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/swaync/" "$pkgdir/etc/skel/.config/"
}

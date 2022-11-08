# Maintainer: KrulYuno <Discord: Lost Felt#8517>
pkgname=krulyuno-system-configs
pkgver=1.1.0
pkgrel=1
pkgdesc="My personal system configs when installing arch for my laptop."
arch=('any')
url="https://github.com/KrulYuno/krulyuno-system-configs"
license=('GPL3')
depends=(
        'acpilight'
        'pipewire'
        'pipewire-alsa'
        'pipewire-jack'
        'pipewire-audio'
        'pipewire-pulse'
)
makedepends=()
backup=(
        'etc/udev/rules.d/90-backlight.rules'
        'etc/X11/xorg.conf.d/30-touchpad.conf'
)
source=()
sha256sums=()

package() {
        install -d "${pkgdir}/etc/udev/rules.d"
        cp -r "${srcdir}/acpilight/90-backlight.rules" "${pkgdir}/etc/udev/rules.d"
        install -d "${pkgdir}/etc/X11/xorg.conf.d"
        cp -r "${srcdir}/X11/30-touchpad.conf" "${pkgdir}/etc/X11/xorg.conf.d"
}

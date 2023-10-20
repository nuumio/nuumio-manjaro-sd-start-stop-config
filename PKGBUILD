pkgname=sd-start-stop-config
pkgver=1.1
pkgrel=1
pkgdesc="Set SCSI disk start and stop managed (spin down on shutdown)"
arch=('any')
url="https://gitlab.com/nuumio-manjaro/sd-start-stop-config"
license=('MIT')
depends=('bash>=5.0.0' 'systemd>=245.0')

source=('sd-start-stop-config'
        'sd-start-stop-config.service')

sha256sums=('SKIP'
            'SKIP')

install=${pkgname}.install

package() {
  install -D "${srcdir}/sd-start-stop-config" "${pkgdir}/usr/bin/sd-start-stop-config"
  install -Dm644 "${srcdir}/sd-start-stop-config.service" "${pkgdir}/usr/lib/systemd/system/sd-start-stop-config.service"
}

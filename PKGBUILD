pkgname=alc298-init
pkgver=1.0
pkgrel=1
pkgdesc="Initialize ALC298 codec using hda-verb"
arch=('x86_64')
url="https://github.com/yorukai/alc298-init"
license=('MIT')
depends=('alsa-utils')
install=
source=(
    'alc298-init.sh'
    'alc298-init.service'
)
sha256sums=('848127ab71f638b12c20695cdb60d71b73d5c7fbbff32311e854543ea6ebcfb8'
            '105099d9aa09bcee3ab5d1ab625e8fda0d2716b297c945f740b1708d90d1d311')

package() {
    install -Dm755 "${srcdir}/alc298-init.sh" \
        "${pkgdir}/usr/bin/alc298-init"

    install -Dm644 "${srcdir}/alc298-init.service" \
        "${pkgdir}/usr/lib/systemd/system/alc298-init.service"
}

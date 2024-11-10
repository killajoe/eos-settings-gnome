# Maintainer: joekamprad <joekamprad at endeavouros.com>

pkgname=eos-settings-gnome
pkgver=2.2
pkgrel=1
pkgdesc="GNOME settings for EndeavourOS"
arch=('any')
url="https://github.com/endeavouros-team/${_pkgname}"
license=('GPL')
makedepends=('git')
source=('99_endeavouros-gnome.gschema.override'
        '98_endeavouros-gnome-console.gschema.override'
        'endeavouros.xml'
        'zz_endeavouros.org.gnome.login-screen.gschema.override')
sha256sums=('d1af9533f50ff30731123e366ab458a2934874313185d820a8f8a088478a6901'
            '07e38ae2006b50e813cfc67021da150597ef88d0efc81147dc5d8955032224f3'
            '1348ecd7bc7445ebb83f062117f6916af23914dbcefca56e4124e99f1ab865b1'
            '58d65a816997c15b5c61cf04586a8faeda076d12c94fc426ee9c2f642f1e5e2e')

package() {
    install -Dm755 "${srcdir}/99_endeavouros-gnome.gschema.override" "${pkgdir}/usr/share/glib-2.0/schemas/99_endeavouros-gnome.gschema.override"
    install -Dm755 "${srcdir}/98_endeavouros-gnome-console.gschema.override" "${pkgdir}/usr/share/glib-2.0/schemas/98_endeavouros-gnome-console.gschema.override"
    install -Dm644 "${srcdir}/endeavouros.xml" "${pkgdir}/usr/share/gnome-background-properties/endeavouros.xml"
    install -Dm755 "${srcdir}/zz_endeavouros.org.gnome.login-screen.gschema.override" "${pkgdir}/usr/share/glib-2.0/schemas/zz_endeavouros.org.gnome.login-screen.gschema.override"
}

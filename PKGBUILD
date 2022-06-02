# Maintainer: Smoque <gbIMoBou@gmail.com>

pkgname=amdgpufan
pkgdesc="amdgpufan"
pkgver=1.0
pkgrel=1
arch=('any')
license=('GPL')
depends=('systemd')

source=('amdgpufan' 'amdgpufan.service' 'amdgpufan.conf')

package(){
    mkdir -p ${pkgdir}/usr/sbin
    cp ${srcdir}/amdgpufan ${pkgdir}/usr/sbin/
    mkdir -p ${pkgdir}/usr/lib/systemd/system
    cp ${srcdir}/amdgpufan.service ${pkgdir}/usr/lib/systemd/system/
    mkdir -p ${pkgdir}/etc
    cp ${srcdir}/amdgpufan.conf ${pkgdir}/etc/default/amdgpufan
}

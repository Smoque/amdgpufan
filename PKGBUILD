# Maintainer: Smoque <gbIMoBou@gmail.com>

pkgname=amdgpufan
pkgdesc="amdgpufan"
pkgver=1.0
pkgrel=1
arch=('any')
license=('GPL')
depends=('systemd')

source=('amdgpufan' 'amdgpufan.service' 'amdgpufan.conf')
sha256sums=('8a0dffacb91331b8de3abe4f4a5bb93a32a994eefb8c55bfc7d6530392fd8a49'
            '2331d59675fd77dabf785a234ba4a0fe4245a1b10ff901f154523a0d56d4fcf1'
            'ecd35c14f71264bbec3ec12c1f2261d92f6ea8a244ac6f5a4aa32dbea52638db')

package(){
    mkdir -p ${pkgdir}/usr/sbin
    cp ${srcdir}/amdgpufan ${pkgdir}/usr/sbin/
    mkdir -p ${pkgdir}/lib/systemd/system
    cp ${srcdir}/amdgpufan.service ${pkgdir}/lib/systemd/system/
    mkdir -p ${pkgdir}/etc
    cp ${srcdir}/amdgpufan.conf ${pkgdir}/etc/default/amdgpufan
}

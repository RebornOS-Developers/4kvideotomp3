# Maintainer: Rafael <rafael@rebornos.org>
# v3.0.1.936

pkgname=4kvideotomp3
pkgver=3.0.1
pkgrel=1
pkgdesc="Convert any video to MP3 in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('3cf78aba06e742516264b7796c2de8fa8c7bc7b4a5ef0b9a941a00c0a325da124a9859b1ce71db00a636f74ef3dae20d13f281cad8e1322534fca7dc191d824f')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}


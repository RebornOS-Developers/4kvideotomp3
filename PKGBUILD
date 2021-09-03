# Maintainer: Rafael <rafael@rebornos.org>
# v3.0.0.930

pkgname=4kvideotomp3
pkgver=3.0.0
pkgrel=1
pkgdesc="Convert any video to MP3 in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('9050c5d6f1a1a9adbfbb49dda8746e8e79fcb5b4529e6e5ebcc929ecdbccecfe73b69da269032ccbcc68fe380c48fa6b0c56f1bd7fb7eaaa941c693f88f8d342')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}


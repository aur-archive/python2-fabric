# Maintainer: Sven-Hendrik Haase <sh@lutzhaase.com>
# Contributor: Francois Boulogne <fboulogne at april dot org>

pkgname=python2-fabric
pkgver=1.6.0
pkgrel=1
pkgdesc="Python library and command-line tool designed to streamline deploying applications or performing system administration tasks via the SSH protocol"
url="http://fabfile.org/"
license=('BSD')
arch=('any')
depends=('python2>=2.5' 'pycrypto' 'python2-paramiko>=1.10.0' 'python2-distribute')
source=("http://pypi.python.org/packages/source/F/Fabric/Fabric-${pkgver}.tar.gz")
md5sums=('e58bde050aad151e3b1b36dbd433f2d7')

build() {
  cd ${srcdir}/Fabric-${pkgver}
  python2 setup.py install --root=${pkgdir} --optimize=1

  install -D -m644 README.rst ${pkgdir}/usr/share/doc/${pkgname}/README.rst
  install -D -m644 LICENSE ${pkgdir}/usr/share/licenses/${pkgname}/LICENSE
}

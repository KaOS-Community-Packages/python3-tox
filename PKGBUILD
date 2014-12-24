pkgname=python3-tox
pkgver=1.8.1
pkgrel=1
pkgdesc='Python virtualenv management and testing tool'
arch=('x86_64')
url='http://testrun.org/tox/latest/'
license=('GPL2')
makedepends=('python3-setuptools' 'python3-py' 'python3-virtualenv')
source=("http://pypi.python.org/packages/source/t/tox/tox-${pkgver}.tar.gz")
sha256sums=('44ca1e038cb57fe40ac0dff8b67b258efe05517bf9b4b4b07035f8be830aac01')

package() {
  cd "$srcdir/tox-$pkgver"
  python3 setup.py build
  python3 setup.py install --root="$pkgdir" --optimize=1
  ln -s tox "${pkgdir}/usr/bin/tox3"
}

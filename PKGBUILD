# Maintainer: Kaiting Chen <kaitocracy@gmail.com>
# Contributor: Michal Krenek <mikos@sg1.cz>

pkgname='flasm'
pkgver='1.62'
pkgrel='2'
pkgdesc='Disassembler tool for SWF bytecode'
arch=('i686' 'x86_64')
url='http://www.nowrap.de/flasm.html'
license=('custom')
depends=('zlib')
makedepends=('gperf')

md5sums=('28a4586409061b385d1cd27d3f120c0b')
source=("http://www.nowrap.de/download/${pkgname}16src.zip")

build() {
  cd "${srcdir}" && make || return 1
  install -Dm755 flasm "$pkgdir/usr/bin/flasm"
  install -Dm644 LICENSE.TXT \
  $pkgdir/usr/share/licenses/$pkgname/LICENSE
}

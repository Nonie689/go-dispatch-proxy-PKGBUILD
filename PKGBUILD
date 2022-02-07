# Maintainer: Nonie689 <nonie689 at eclipso dot ch>
pkgname=go-dispatch-proxy-git
pkgver=5.0.0
pkgrel=1
pkgdesc="A SOCKS5 load balancing proxy to combine multiple internet connections into one"
arch=('i686' 'x86_64')
url="https://github.com/extremecoders-re/go-dispatch-proxy"
license=('GPL')
makedepends=("go")
install=
source=("git+https://github.com/extremecoders-re/go-dispatch-proxy.git")
md5sums=()

build() {
  cd "$srcdir/$pkgname"

  go build
}

package() {
  cd "$srcdir/$pkgname"

  make DESTDIR="$pkgdir/" install
}

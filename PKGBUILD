pkgname='win32yank'
pkgver='0.0.4'
pkgrel=1
arch=('x86_64')
pkgdesc='Windows clipboard tool'
makedepends=('unzip=6.0-15')
source=("https://github.com/equalsraf/$pkgname/releases/download/v$pkgver/$pkgname-x64.zip")
sha512sums=('782384302bd456b0dd3e422bbb53b88d2ffda0cb423d942a669a348f9fcb22c8e2141952e69b7260d736e8c275c504f0e5816268644452f892a2c716f5e53776')

package() {
  mkdir -p "$pkgdir/usr/local/bin"
  unzip -p "$srcdir/$pkgname-x64.zip" "$pkgname.exe" > "$pkgdir/usr/local/bin/$pkgname.exe"
  chmod +x "$pkgdir/usr/local/bin/$pkgname.exe"
}


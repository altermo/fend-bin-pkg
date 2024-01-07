pkgname=fend-bin
pkgver=1.4.1
pkgrel=1
pkgdesc="Arbitrary-precision unit-aware calculator"
arch=('x86_64')
url="https://github.com/printfn/fend"
license=('MIT')
provides=('fend')
conflicts=('fend')
source=("https://raw.githubusercontent.com/printfn/fend/v$pkgver/LICENSE.md"
        "https://github.com/printfn/fend/releases/download/v$pkgver/fend.1")
source_x86_64=("$pkgname-$pkgver-x86_64.tar.gz::https://github.com/printfn/fend/releases/download/v$pkgver/fend-$pkgver-linux-x64.zip")
sha256sums=('cc5470feed66192387f06ae93aed0bd4fefae5a5fd7c1e54a4acf4ea64f1028b'
            '4296b44f1d290125cf43114d4556c3cde1c4124e979a83f6aeb3e924678ed362')
sha256sums_x86_64=('a68f0324be2f21efa706c37a03d7fd017cfab5c33e74f7d0e117512cf7814f5f')

package() {
  install -Dm755 fend -t "$pkgdir/usr/bin"
  install -Dm644 LICENSE.md "$pkgdir/usr/share/licenses/fend/LICENSE"
  install -Dm644 fend.1 -t "$pkgdir/usr/share/man/man1"
}

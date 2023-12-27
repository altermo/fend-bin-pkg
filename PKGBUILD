pkgname=fend-bin
pkgver=1.4.0
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
            'b2a23e220473a9151f76bf18dc27c94ccc09afe4b7eacb49848d0a181bfdee38')
sha256sums_x86_64=('9b2db780866a2617f904fb47af3a927bb77833865dd32f520f2954eda0dcc77f')

package() {
  install -Dm755 fend -t "$pkgdir/usr/bin"
  install -Dm644 LICENSE.md "$pkgdir/usr/share/licenses/fend/LICENSE"
  install -Dm644 fend.1 -t "$pkgdir/usr/share/man/man1"
}

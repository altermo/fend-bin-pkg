# Maintainer: Funami
pkgname=fend-bin
pkgver=1.3.2
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
sha256sums=('a59abf360ab4ce1ce88d0c73f872313da3e6c5894799357a8423d6b68d966c43'
            '00383f830389634c9634cc4731692950422c71071ca55e691ae28c9bbe7b056a')
sha256sums_x86_64=('9dddd9ed2704e8eede5d58d28c41e32a279c7e2aca829869ec1647785a0fff40')

package() {
  install -Dm755 fend -t "$pkgdir/usr/bin"
  install -Dm644 LICENSE.md "$pkgdir/usr/share/licenses/fend/LICENSE"
  install -Dm644 fend.1 -t "$pkgdir/usr/share/man/man1"
}

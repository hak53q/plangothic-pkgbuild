# Maintainer: hak53q <hak53q@gmail.com>

pkgname=otf-plangothic
pkgver=2.9.5779
pkgrel=1
arch=(any)
url='https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project'
license=(OFL)
depends=('fontconfig' 'unzip')
source=(
  Plangothic-OTF-V$pkgver.zip::"https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project/releases/download/V$pkgver/Plangothic-OTF-V$pkgver.zip"
)
sha256sums=(
  '8439ff2b89f313322780c8c4ac57f2df94b632ee53531ab3e8abaacb88ef72b6'
)

package() {
  unzip -u $srcdir/Plangothic-OTF-V$pkgver.zip
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP1-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP1-Regular.otf"
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP2-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP2-Regular.otf"
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/LICENSE.txt" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

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
  'b19f8514a6c33ca67c89eea5dd4f8f816c3346535f88c0c1184e445c8043fca5'
)

package() {
  unzip -u $srcdir/Plangothic-OTF-V$pkgver.zip
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP1-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP1-Regular.otf"
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP2-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP2-Regular.otf"
#  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/LICENSE.txt" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

# Maintainer: hak53q <hak53q@gmail.com>

pkgname=otf-plangothic
pkgver=2.9.5779
pkgrel=1
arch=(any)
url='https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project'
license=(OFL)
depends=('fontconfig' '7zip')
source=(
  Plangothic-OTF-V$pkgver.7z::"https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project/releases/download/V$pkgver/Plangothic-OTF-V$pkgver.7z"
  LICENSE::"https://raw.githubusercontent.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic_Project/refs/heads/main/LICENSE.txt"
)
sha256sums=(
  '1139867931a1cdfc7777a755824be5f31c79b0fc9f42d545f6f57981fa2119ba'
  'e564f06d018e7b95bc3594c96a17f1d41865af4038c375e7aa974dd69df38602'
)

package() {
  7z x -aoa $srcdir/Plangothic-OTF-V$pkgver.7z
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP1-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP1-Regular.otf"
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP2-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP2-Regular.otf"
  install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
  install -Dm644 "$srcdir"/56-otf-plangothic.conf -t /usr/share/fontconfig/conf.avail/
  ln -s /usr/share/fontconfig/conf.avail/56-otf-plangothic.conf /usr/share/fontconfig/conf.default/
}

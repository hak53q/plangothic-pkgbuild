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
  56-otf-plangothic-p1.conf::"https://raw.githubusercontent.com/hak53q/plangothic-pkgbuild/refs/heads/main/56-otf-plangothic-p1.conf"
  56-otf-plangothic-p2.conf::"https://raw.githubusercontent.com/hak53q/plangothic-pkgbuild/refs/heads/main/56-otf-plangothic-p2.conf"
)
sha256sums=(
  '4e5ae828f14f2805a159ca298d03df107b8788da5e8bc22b53e1767dbf873a9f'
  'e564f06d018e7b95bc3594c96a17f1d41865af4038c375e7aa974dd69df38602'
  '69932f0b1ed9248b11a378ae39697329c4733bc7ff24d247f4642015ba00e4a4'
  '70f634fe2e1c9d20d03bc14ff41a24e1e425db1a633b7552b5b153ef0dafa860'
)

package() {
  7z x -aoa $srcdir/Plangothic-OTF-V$pkgver.7z
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP1-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP1-Regular.otf"
  install -Dm644 "$srcdir/Plangothic-OTF-V$pkgver/PlangothicP2-Regular.otf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP2-Regular.otf"
  install -Dm644 "$srcdir/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
  install -Dm644 "$srcdir/56-otf-plangothic-p1.conf" "${pkgdir}/etc/fonts/conf.d/56-otf-plangothic-p1.conf"
  install -Dm644 "$srcdir/56-otf-plangothic-p2.conf" "${pkgdir}/etc/fonts/conf.d/56-otf-plangothic-p2.conf"
}

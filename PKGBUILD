pkgname=ttf-plangothic
pkgver=1.9.5769
pkgrel=1
pkgdesc='遍黑体项目（Plangothic Project）'
arch=(any)
url='https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project'
license=(OFL)
depends=(fontconfig)
source=(
  PlangothicP1-Regular-$pkgver.ttf::"https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project/releases/download/V$pkgver/PlangothicP1-Regular.fallback.ttf"
  PlangothicP2-Regular-$pkgver.ttf::"https://github.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic-Project/releases/download/V$pkgver/PlangothicP2-Regular.ttf"
  $pkgname-LICENSE::"https://raw.githubusercontent.com/Fitzgerald-Porthmouth-Koenigsegg/Plangothic/V$pkgver/LICENSE"
)
sha256sums=(
  '299f2a5556281a68c67bd9abcbc45d6662b48e2da620e611f8156a9119bea839'
  'a575a268b3ae456e0fded01f2fe22bf44b4748fa2f57cd6e5cf9e243b0470180'
  '15d798b5ba1e746b3789dea9457957af2f4c3f56849f09de7ebd35457738c14e'
)

package() {
  install -Dm644 "$srcdir/PlangothicP1-Regular-$pkgver.ttf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP1-Regular.ttf"
  install -Dm644 "$srcdir/PlangothicP2-Regular-$pkgver.ttf" "$pkgdir/usr/share/fonts/plangothic/PlangothicP2-Regular.ttf"
  install -Dm644 "$srcdir/$pkgname-LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}

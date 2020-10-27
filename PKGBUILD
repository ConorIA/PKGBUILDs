# Maintainer: Fabien LEFEBVRE <contact@d1ceward.com>

pkgname=procfile-util
pkgver=0.11.0
pkgrel=1
pkgdesc='A tool for interacting with Procfiles.'
arch=('x86_64')
url='https://github.com/josegonzalez/go-procfile-util'
license=('MIT')

source=("https://github.com/josegonzalez/go-procfile-util/releases/download/v${pkgver}/procfile-util_${pkgver}_linux_x86_64.tgz"
        'LICENSE')
sha256sums=('c40dd81ec7ad0efbd00339262b4cb593da361f6214ecbff84cf145c59baa5414'
            '725569065205b55f534d4b040428cef585720756fd953fbdf1a055b6c3349321')

package() {
  install -Dm 755 procfile-util "${pkgdir}/usr/bin/procfile-util"
  install -Dm644 LICENSE "${pkgdir}/usr/share/licenses/procfile-util/LICENSE"
}

# Maintainer: Your Name <vinayakg236@gmail.com>
pkgname=PROClient
pkgver=1.0.0
pkgrel=1
pkgdesc="PROClient for Linux (binary-only release)"
arch=('x86_64')
url="https://"
license=('custom')
options=('!debug')

depends=('glibc')  # Add more if needed
source=("PROClient_linux.tar.gz"
        "proclient.desktop")
sha256sums=('SKIP' 'SKIP')  # Replace with actual checksums if desired

package() {
  cd "$srcdir"

  # Install everything into /opt/PROClient
  install -d "$pkgdir/opt/PROClient"
  cp -r ./* "$pkgdir/opt/PROClient"

  # Install the .desktop file
  install -Dm644 proclient.desktop "$pkgdir/usr/share/applications/proclient.desktop"

  # Optional: Symlink to /usr/bin
  install -d "$pkgdir/usr/bin"
  ln -sf /opt/PROClient/PROClient_x86 "$pkgdir/usr/bin/proclient"
}

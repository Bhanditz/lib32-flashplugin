pkgname=lib32-flashplugin
pkgver=11.2.202.270
pkgrel=1
license=('custom')
pkgdesc='Adobe Flash Player for 32-bit Mozilla-based browsers'
url="http://get.adobe.com/flashplayer"
arch=('x86_64')
depends=('mozilla-common' 'lib32-libxt' 'lib32-gtk2' 'lib32-nss' 'lib32-curl' 'lib32-alsa-lib')
optdepends=('lib32-libvdpau: video hardware decoding for supporting players'
            'nspluginwrapper: make this plugin work with 64-bit browsers'
            'bin32-firefox: 32-bit Firefox for 64-bit systems')
options=(!strip)
source=("flashplugin-${pkgver}.i386.tar.gz::http://fpdownload.macromedia.com/get/flashplayer/pdc/${pkgver}/install_flash_player_11_linux.i386.tar.gz")

md5sums=('67ffda3effdf937eaed48a46f2f6f21a')

build() {
  install -Dm644 "${srcdir}/libflashplayer.so" "${pkgdir}/usr/lib32/mozilla/plugins/libflashplayer.so"
}


# Maintainer: Dwayne Bent <me@dwayne.bent.io>

pkgname=luaevent
pkgver=0.4.1
pkgrel=2
pkgdesc="libevent binding for Lua"
arch=('i686' 'x86_64')
url="https://github.com/harningt/luaevent"
license=('LGPL2.1')
depends=('libevent>=1.4' 'lua-socket' 'lua>=5.1')
source=($pkgname-$pkgver.tar.gz::https://github.com/harningt/luaevent/tarball/v$pkgver)
sha512sums=('60b4184cd34794cea04eefe7cabcf4efdaa4389d1ce79589a3bb95dafde8f228e57abe3bb8dd7f434d172f3618d200d09176721f69386be25d59ee62c5b73824')

build() {
    cd "$srcdir/harningt-$pkgname"*
    make
}

package() {
    cd "$srcdir/harningt-$pkgname"*
    make DESTDIR="$pkgdir" install
}


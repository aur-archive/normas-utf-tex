# Maintainer: Igor Ramos Tiburcio <irtigor@yahoo.com.br>
# Contributor: Fabiano Rosas

pkgname='normas-utf-tex'
pkgver='3.1'
pkgrel=2
pkgdesc="A LaTeX class for writing documents in UTF standard"
arch=(any)
url="http://sourceforge.net/projects/normas-utf-tex/"
license=('GPL3')
depends=('abntex')
install=$pkgname.install
provides=(normas-utf-tex)
source=(http://downloads.sourceforge.net/project/normas-utf-tex/versao-com-dependencias/"$pkgname"-com-dependencias-utf8-"$pkgver".tar.bz2)
md5sums=('dd81ad3b513009cf608a1c212288b476')

package() {
  install -D -m 644 "$pkgname"-com-dependencias-utf8-"$pkgver"/"$pkgname".cls $pkgdir/usr/share/texmf/tex/latex/"$pkgname"/"$pkgname".cls
  install -d -m 755 $pkgdir/usr/share/texmf/doc/"$pkgname"
  cp -r "$pkgname"-com-dependencias-utf8-"$pkgver"/exemplos/* $pkgdir/usr/share/texmf/doc/"$pkgname"
}

# vim:set ts=2 sw=2 et:

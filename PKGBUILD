# Contributor: Christian Hausknecht <christian.hausknecht@gmx.de>
# http://downloads.sourceforge.net/project/simutrans/pak.german/pak64.german-110-0c/simupak-german64-110-0c.zip

pkgname=simutrans-pak64-german
pkgver=110
_pkgver=$pkgver-0c
pkgrel=1
pkgdesc="A graphics set for Simutrans with german settings"
arch=(any)
url="http://www.simutrans.com/paksets.htm#pak64.German"
license=('custom:Artistic License')
depends=('simutrans>=111.2')
provides=("simutrans-pak64-german=$_pkgver")
options=(!strip)
source=(http://downloads.sourceforge.net/project/simutrans/pak.german/pak64.german-110-0c/simupak-german64-110-0c.zip
        LICENSE.txt)
md5sums=(f29fb4a48c429cee6e59ce53317da470
        88f7c4912aebe9740e31585406f2bf7b)

package() {
  cd "$srcdir"

  #data
  mkdir -p "$pkgdir/usr/share/games/simutrans"
  cp -r simutrans/pak64.german "$pkgdir/usr/share/games/simutrans"

  #license
  install -Dm644 LICENSE.txt "$pkgdir/usr/share/licenses/$pkgname/LICENSE.txt"
}

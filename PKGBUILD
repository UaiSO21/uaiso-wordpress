# Mantenedor  : Maurício de Lima <mauricio@uai21.com>
# Website     : https://uaiso.uai21.com

pkgname=uaiso-wordpress
pkgver=6.1.1
pkgrel=1
pkgdesc='Software de gerenciamento de conteúdo (CMS) muito utilizado em blogs'
arch=(any)
url='https://wordpress.org/'
license=(GPL)

depends=('php'
         'php-imagick
         'php-gd'
         'mariadb'
         )

optdepends=('apache: Servidor Web'
            'nginx: Servidor Web')

options=(emptydirs)
install=$pkgname.install
source=("https://wordpress.org/wordpress-$pkgver.tar.gz")
b2sums=('fbbee51219e4237236c39255deb9e31e566c630cfc66f0c4744fec249ae1d07473a6222b7ec5d84079e616d8d2e790521e57809d357ab56582b4a292dbad82f1')

package() {
  install -d "$pkgdir/srv/http"
  cp -r wordpress "$pkgdir/srv/http"
}

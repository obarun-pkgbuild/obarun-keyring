# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-keyring
pkgver=20171127
pkgrel=1
pkgdesc='Obarun PGP keyring'
arch=('x86_64')
url='https://obarun.org/'
install="${pkgname}.install"
source=('Makefile'
		'obarun.gpg'
		'obarun-revoked'
		'obarun-trusted')
md5sums=('110e310b896c8ee085b71e71bfc853f8'
         '6ff4a7bb1ff9acdccf4515337cbc0df6'
         'd41d8cd98f00b204e9800998ecf8427e'
         'e30c98e1fbdb267bd2b23318956dbb18')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC' # Eric Vidal
			'EE62628C5670B472C1529563D4CA511F0375F9B2') # Danial Spruce

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}

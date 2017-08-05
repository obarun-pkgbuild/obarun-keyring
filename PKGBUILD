# Maintainer: Eric Vidal <eric@obarun.org>

pkgname=obarun-keyring
pkgver=20161209
pkgrel=2
pkgdesc='Obarun PGP keyring'
arch=('any')
url='https://obarun.org/'
install="${pkgname}.install"
source=('Makefile'
		'obarun.gpg'
		'obarun-revoked'
		'obarun-trusted')
md5sums=('110e310b896c8ee085b71e71bfc853f8'
         '09a4e55c1b7b646751d058520e1ac8e4'
         'd41d8cd98f00b204e9800998ecf8427e'
         'baff696de97dd15b2cb1eb67be9914a0')
validpgpkeys=('6DD4217456569BA711566AC7F06E8FDE7B45DAAC' # Eric Vidal
			'EE62628C5670B472C1529563D4CA511F0375F9B2') # Danial Spruce

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}

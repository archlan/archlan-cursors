# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    PKGBUILD                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: Lanhild <archlan@protonmail.com>           +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/01/16 20:35:29 by Lanhild           #+#    #+#              #
#    Updated: 2022/01/16 20:36:17 by Lanhild          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

pkgname=archlan-cursor-material
pkgver=1.0
pkgrel=1
pkgdesc="Cursor theme for ArchLan"
url="https://github.com/archlan/archlan-cursors"
arch=('any')
license=('GPL3')
makedepends=()
depends=()
conflicts=()
groups=(archlan-cursors)
provides=("${pkgname}")
options=(!strip !emptydirs)

prepare() {
	cp -af ../files/. ${srcdir}
}

package() {
	local _cursorsdir=${pkgdir}/usr/share/icons
	mkdir -p "$_cursorsdir"
	cp -r ${srcdir}/* "$_cursorsdir"
}
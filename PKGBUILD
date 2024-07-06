
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Jacob Stannix <jakestannix@gmail.com>
pkgname=rguilayout
pkgver=4.0
pkgrel=2
epoch=
pkgdesc="A simple and easy-to-use raygui layouts editor"
arch=(x86_64)
url="https://github.com/raysan5/rguilayout"
license=('ZLIB')
groups=(raygui-dev)
depends=("raygui>=4.0")
makedepends=()
checkdepends=()
optdepends=()
provides=(rguilayout=4.0)
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("https://github.com/raysan5/rguilayout/releases/download/${pkgver}/${pkgname}_v${pkgver}_linux_x64.zip")
noextract=()
sha256sums=(efc30608b21689f7b077932af83227ff6e47bf9c24b81ef7f28adf91accf62a1)
validpgpkeys=()

prepare() {
	cd "${pkgname}_v${pkgver}_linux_x64"

}

build() {
	cd "${pkgname}_v${pkgver}_linux_x64"
	
}

package() {

	cd "${pkgname}_v${pkgver}_linux_x64"

	mkdir -p "$pkgdir/usr/share/rguilayout/layouts"
	mkdir -p "$pkgdir/usr/bin/"
	install -m644 -t "$pkgdir/usr/share/rguilayout/layouts/"\
		"layouts/window_audio_player.rgl"\
		"layouts/window_file_dialog.rgl"\
		"layouts/window_image_edit.rgl"\
		"layouts/window_image_export.rgl"\
		"layouts/window_image_import_raw.rgl"\
		"layouts/window_image_resize.rgl"\
		"layouts/window_messagebox.rgl"
	install -m644 -t "$pkgdir/usr/share/rguilayout" \
		"README.md"\
		"USAGE.md"
	install -m755 -t "$pkgdir/usr/bin/" "$pkgname"

}


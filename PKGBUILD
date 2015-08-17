# Maintainer: Andreas B. Wagner <AndreasBWagner@pointfree.net>
# Maintainer: Sascha Biermanns <http://prprivacybox.de/saschakb.msg>
# Contributor: Robson R S Peixoto <robsonpeixoto@gmail.com>

pkgname=vim-clang-complete
pkgver=2.0
_scriptid=19588
pkgrel=2
pkgdesc='clang complete : Use of Clang for completing C, C++, Objective-C and Objective-C++'
arch=('any')
url='http://www.vim.org/scripts/script.php?script_id=3302'
license=('unknown')
depends=('vim' 'clang>2.9')
conflicts=('vim-omnicppcomplete')
source=("clang_complete.vmb::http://www.vim.org/scripts/download_script.php?src_id=$_scriptid")
install=vimdoc.install
md5sums=('44ec52af1184fb1cc3465cd6c612a333')

build() {
  cd "$srcdir"
  mkdir -p ${pkgdir}/usr/share/vim/vimfiles
  vim -c "UseVimball ${pkgdir}/usr/share/vim/vimfiles" -c "q" clang_complete.vmb
  rm ${pkgdir}/usr/share/vim/vimfiles/doc/tags
}

# vim:set ts=2 sw=2 et:

# SPDX-License-Identifier: AGPL-3.0
#
# Maintainer: Truocolo <truocolo@aol.com>
# Maintainer: Pellegrino Prevete (tallero) <pellegrinoprevete@gmail.com>
# Maintainer: Malachi Soord <me@malachisoord.com>

_pkg=asciinema-edit
pkgname="${_pkg}-bin"
pkgver=0.0.6
pkgrel=1
pkgdesc="asciinema casts post-production tools."
_http="https://github.com"
_ns="cirocosta"
url="https://github.com/${_ns}/${_pkg}"
arch=(
  'x86_64'
)
license=(
  'MIT'
)
provides=(
  "${_pkg}=${pkgver}"
)
conflicts=(
  "${_pkg}"
)
_bin="${url}/releases/download/${pkgver}/${_pkg}_${pkgver}_linux_amd64.tar.gz"
source=(
  "${_bin}"
)
sha512sums=(
  'd99dac29a22532b3558ae59d8dfcfe08a227d64f10de4dda3be7cd17052ff303c12745d5a46fac269a9df143feb67c28b015bbadaa6f87d6f03b39193deca9a5')

package() {
  install \
    -Dm755 \
    "${_pkg}" \
    "${pkgdir}/usr/bin/${_pkg}"
  install \
    -Dm644 \
    "LICENSE" \
    "${pkgdir}/usr/share/licenses/${pkgname}"
  install \
    -Dm644 \
    "README.md" \
    "${pkgdir}/usr/share/doc/${pkgname}/README.md"
}


pkgname=ttf-material-symbols-variable
pkgver=4_0_0
pkgrel=1
pkgdesc="Google Material Symbols icon set"
arch=('any')
license=('Apache License 2.0')
url="https://github.com/google/material-design-icons"
_branche="master"
source=("MaterialSymbolsOutlined-${pkgver}.ttf::https://github.com/google/material-design-icons/raw/${_branche}/variablefont/MaterialSymbolsOutlined%5BFILL,GRAD,opsz,wght%5D.ttf"
	"MaterialSymbolsRounded-${pkgver}.ttf::https://github.com/google/material-design-icons/raw/${_branche}/variablefont/MaterialSymbolsRounded%5BFILL,GRAD,opsz,wght%5D.ttf"
	"MaterialSymbolsSharp-${pkgver}.ttf::https://github.com/google/material-design-icons/raw/${_branche}/variablefont/MaterialSymbolsSharp%5BFILL,GRAD,opsz,wght%5D.ttf"
	"${pkgname}-${pkgver}-LICENSE::https://github.com/google/material-design-icons/raw/${_branche}/LICENSE")
sha256sums=('1a8da11650a6f49b22152c48dec37803c9aa94b0ba49c4ef6d8e95cdde1ce982'
            '4c13567021e456fa546c79afd54b4adf89ecf3e37380db7df272fcf238302dc3'
            'a767a745765ad61254b93c56a4b8f92b02d3626a3ba09412443b000e65524665'
            '58d1e17ffe5109a7ae296caafcadfdbe6a7d176f0bc4ab01e12a689b0499d8bd')
	
package() {
	install -dm 755 "${pkgdir}/usr/share/fonts/material-design-icons"
	install -m 644 MaterialSymbolsOutlined-${pkgver}.ttf "${pkgdir}/usr/share/fonts/material-design-icons/MaterialSymbolsOutlined.ttf "
	install -m 644 MaterialSymbolsRounded-${pkgver}.ttf "${pkgdir}/usr/share/fonts/material-design-icons/MaterialSymbolsRounded.ttf"
	install -m 644 MaterialSymbolsSharp-${pkgver}.ttf "${pkgdir}/usr/share/fonts/material-design-icons/MaterialSymbolsSharp.ttf"
	install -Dm644 ${pkgname}-${pkgver}-LICENSE "${pkgdir}/usr/share/licenses/$pkgname/LICENSE"
}

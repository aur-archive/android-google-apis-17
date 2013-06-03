# Maintainer: Joel Pedraza <joel@joelpedraza.com>
# Contributor: Jakub Schmidtke <sjakub-at-gmail-dot-com>

_rev=r03
_sdkver=4.2.2
_sdkint=17
pkgname=android-google-apis-${_sdkint}
pkgver=${_sdkver}_${_rev}
pkgrel=1
pkgdesc="Android Google APIs, API-${_sdkint}"
arch=('any')
url="http://code.google.com/android/add-ons/google-apis"
license=('custom')
depends=("android-platform-${_sdkint}")
options=('!strip')
source=("http://dl.google.com/android/repository/google_apis-${_sdkint}_${_rev}.zip")
sha1sums=('8246f61d24f0408c8e7bc352a1e522b7e2b619ba')
package() {
  mkdir -p "${pkgdir}/opt/android-sdk/add-ons/"
  mv "${srcdir}/google_apis-671458-mac-x86" "${pkgdir}/opt/android-sdk/add-ons/addon-google_apis-google_inc_-${_sdkint}"

  chmod -R ugo+rX "${pkgdir}/opt"
}

# Maintainer: alex4ip <alex4ip@gmail.com>
# Contiributer: Alex Ellis <alex@openfaas.com>

pkgname=k3sup-bin
_pkgname=k3sup
pkgver=0.9.7
pkgrel=1
epoch=1
pkgdesc='k3sup is a light-weight utility to get from zero to KUBECONFIG with k3s on any local or remote VM.'
arch=(x86_64)
url='https://github.com/alexellis/k3sup/'
license=(MIT)
depends=('openssh')
#depends=('docker')
optdepends=('k3s'
            'kubernetes-bin'
            'helm'
            'terraform'
            'azure-cli: Command-line tools for Azure'
            'aws-cli: cli for Amazon Web Services'
            'google-cloud-sdk: gcloud - command-line tools for the Google Cloud Platform')
provides=('k3sup')
#makedepends=('go')
_OWNER=alexellis
_suffix=""
source=("$pkgname-$pkgver::https://github.com/${_OWNER}/${_pkgname}/releases/download/${pkgver}/${provides}${_suffix}")
sha256sums=('9bde60a27364e5cdd6021b03b3f6bad7d385e6651c9956a280fe86f6e4e8e678')

package() {  
  #mkdir -p "${pkgdir}/opt"
  install -Dm 755 "$srcdir/$pkgname-$pkgver" "${pkgdir}/usr/local/bin/${provides}"

  # mkdir -p "${pkgdir}/usr/local/bin"
  # ln -nfs /opt/${pkgname}/${provides} "${pkgdir}"/usr/local/bin/${provides}

  # Add command completion
  # install -dm 755 "$pkgdir/usr/share/bash-completion/completions"
  # install -dm 755 "$pkgdir/usr/share/zsh/site-functions"
  # "$pkgdir/usr/bin/provides" completion bash > "$pkgdir/usr/share/bash-completion/completions/provides"
  # "$pkgdir/usr/bin/provides" completion zsh >  "$pkgdir/usr/share/zsh/site-functions/_provides"
}

# vim:set ts=2 sw=2 et:

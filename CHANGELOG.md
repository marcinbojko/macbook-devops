# Changelog

## Version 0.5.5

* Fixed differences in packages between arm64 and amd64 architectures
* Tested under real arm64 Macbook architecture
* fixed wrong variable name for arm64 architecture links in `download_files` task
* added `npm` packages section
* [SOFTWARE] added `rosetta2` optional install
* [FORMULA] added `qemu`
* [FORMULA] added `datree`
* [CASKS] added `firefox`
* [CASKS] added `enpass`
* [APPLICATION] bump `kubestr` to version 0.4.33

## Version 0.5.0

* [CASKS] added `wpsoffice` - [https://www.wps.com/](https://www.wps.com/)
* [FORMULA] added `links`
* [FORMULA] added `asciinema`
* [FORMULA] added `imagemagick`
* [FORMULA] added `syft` - [https://github.com/anchore/syft](https://github.com/anchore/syft)
* [FORMULA] added `trivy` - [https://github.com/aquasecurity/trivy](https://github.com/aquasecurity/trivy)
* [TAPS] added `homebrew_taps` section in variables
* [TAPS] added `anchore/syft`

## Version 0.4.0

* added more packages to be in sync with [https://github.com/marcinbojko/linux_mint](https://github.com/marcinbojko/linux_mint)
* introduced separation for `x86_64` and `arm64` architecture

## Version 0.3.0

* [FORMULA] added krew [https://github.com/kubernetes-sigs/krew](https://github.com/kubernetes-sigs/krew)
* [FORMULA] added k3sup [https://github.com/alexellis/k3sup](https://github.com/alexellis/k3sup)
* [FORMULA] added `arping`
* [FORMULA] added `esolitos/ipa/sshpass`
* [APPLICATION] added `dockle` - container image linter [https://github.com/goodwithtech/dockle](https://github.com/goodwithtech/dockle)
* [APPLICATION] added `polaris` [https://github.com/FairwindsOps/polaris](https://github.com/FairwindsOps/polaris)
* [FORMULA] added `minikube`

## Version 0.2.0

* added more packages to be in sync with [https://github.com/marcinbojko/linux_mint](https://github.com/marcinbojko/linux_mint)
* added pip modules section

## Version 0.1.0

* added `update_homebrew` variable to update homebrew itself
* added `update_homebrew_packages` to update installed bre formulae and casks
* added `download_files.yml` task which will handle files being available as archives
  * added `unpack_folder` variable for a task
  * added `bin_path` variable for a task
* added `kubestr` to downloaded packages

## Versions 0.0.1-0.0.3

* Initial commits

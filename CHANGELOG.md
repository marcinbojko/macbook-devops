# Changelog

## Version 0.8.3

* [FORMULA] added `shellcheck`
* [CASK] added `chatgpt`
* [CASK] added `double-commander`

## Version 0.8.2

* [FIX] fixed error for `upgrade_homebrew_packages` variable not being used
* [FORMULA] rename `esolitos/ipa/sshpass` to `sshpass`
* [FORMULA] added `micro` [https://github.com/zyedidia/micro](https://github.com/zyedidia/micro)
* [FORMULA] added `eza` [https://github.com/eza-community/eza](https://github.com/eza-community/eza)
* [FORMULA] added `duf` [https://github.com/muesli/duf](https://github.com/muesli/duf)
* [FORMULA] added `act` [https://github.com/nektos/act](https://github.com/nektos/act)
* [FORMULA] added `yq`
* [CASK] added `karabine-elements` [https://karabiner-elements.pqrs.org/](https://karabiner-elements.pqrs.org/)
* [CASK] added `alfred` [https://www.alfredapp.com/](https://www.alfredapp.com/)
* [CASK] added `iina` [https://iina.io/](https://iina.io/)
* [APPLICATION] upgraded `polaris` to version 9.1.1
* [APPLICATION] upgraded `kubestr` to version 0.4.44

## Version 0.8.1

* [TAPS] added `spectralops/tap`
* [FORMULA] added `spectralops/tap/teller`
* [CASKS] added added `headlamp`
* [CASKS] added `openlens`

## Version 0.8.0

* [ALIBABA] added `alibaba-cloud`
* [ALIBABA] added `aliyun-cli`
* [TAPS] added `hashicorp/tap`
* [FORMULA] added `terraform`
* [FORMULA] added `packer`
* [FORMULA] added `vault`
* [CASKS] removed `synergy-core`
* [APPLICATION] upgraded `polaris` to version 9.0.1
* [APPLICATION] upgraded `dockle` to version 0.4.14
* [APPLICATION] switch `kubent` to homebrew version
* variable `update_homebrew_packages` renamed `upgrade_homebrew_packages`

## Version 0.7.0

* [APPLICATION] upgraded `kubestr` to version 0.4.41
* [APPLICATION] upgraded `polaris` to version 8.4.0
* [APPLICATION] upgraded `dockle` to version 0.4.13
* [APPLICATION] upgraded `kubent` to nightly-0.7.0-33-gdf9a017
* [APPLICATION] removed `skaffold`
* [APPLICATION] added `csshx`
* [APPLICATION] added `k9s`
* [APPLICATION] added `qemu`
* [APPLICATION] added `siege`
* [APPLICATION] added `smartmontools`
* [APPLICATION] added `terminator`
* [APPLICATION] added `s3cmd`
* [CASKS] removed `hamsket-nightly`
* [CASKS] removed `virtualbox-extension-pack`
* [CASKS] added `microsoft-teams`
* [CASKS] added `vagrant`
* [CASKS] added `rambox`

## Version 0.6.2

* [CASKS] removed `ksnip`
* [CASKS] removed `ccleaner`
* [CASKS] added `shottr`
* [CASKS] added `onyx`

## Version 0.6.1

* [CASKS] added `remote-desktop-manager-free`
* [CASKS] added `angry-ip-scanner`
* [CASKS] added `zulu17`
* [FORMULA] added `steampipe` [https://github.com/turbot/steampipe](https://github.com/turbot/steampipe)
* [TAPS] added turbot/tap

## Version 0.6.0

* added possibility to set osx_defaults through `osx_defaults` module
* added variable `install_osx_defaults`
* added variable `install_appstore`
* [APPLICATION] upgraded `kubestr` to version 0.4.34
* [APPLICATION] upgraded `polaris` to version 7.0.1
* [APPLICATION] upgraded `kubent` `nightly-0.5.1-25-g2321172`

## Version 0.5.6

* [CASKS] added `ksnip`
* [CASKS] added `kvlc`
* [CASKS] added `ccleaner`
* [CASKS] added `enpass`
* [CASKS] added `calibre`
* [CASKS] added `utm`
* [CASKS] added `numi`
* [CASKS] added `parallels-virtualization-sdk`
* [FORMULA] added `mas`
* added possibility to install AppStore Applications through playbook

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

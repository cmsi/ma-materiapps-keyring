materiapps-keyring
==================

GPG public key of MateriApps LIVE! debian package repository.

## How to build materiapps-keyring package

1. パッケージのビルド

        sh $HOME/vagrant/development/ma-materiapps-keyring/host-build.sh

2. パッケージへの署名

        sh $HOME/vagrant/development/ma-materiapps-keyring/host-sign.sh

3. リポジトリへの登録

        sh $HOME/vagrant/development/MateriAppsLive/repos/host-add.sh materiapps-keyring

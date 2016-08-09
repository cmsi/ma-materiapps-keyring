materiapps-keyring
==================

GPG public key of MateriApps LIVE! debian package repository.

## How to build materiapps-keyring package

1. ビルドディレクトリの準備

        cd $HOME/build
        sh /development/ma-materiapps-keyring/setup.sh

2. パッケージのビルド

        cd $HOME/build
        sh /development/ma-materiapps-keyring/build.sh 2>&1 | tee build.log

3. パッケージへの署名

        cd $HOME/build
        debsign materiapps-keyring_*.changes 

4. リポジトリへの登録

        cd $HOME/build
        sh /development/MateriAppsLive/repos/add_repo.sh materiapps-keyring_*.changes

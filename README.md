# Let's Encrypt!  のセットアップスクリプト


## 概要  
Let's Encrypt!
[https://letsencrypt.jp/]
のセットアップスクリプトです。
「certbotインストール」⇛「証明書発行」⇛「Apacheに適用」⇛「cronに自動更新登録」を行います。


## 環境
普段DockerベースでWebサーバを運用しており、ベースイメージはDebian(Stretch)+Apache2です。今回はこれがターゲットです。   

### Debian + Apache2 + certbot 
*  Debian(Stretch) 9.6
*  Apache2   2.4.10
*  certbot 0.10.2

### Dockerイメージ  
使ったのは、`php:7.1.24-apache-stretch` です。元イメージは、`debian:stretch-slim` です。

## 実行方法
環境設定ファイル(.env)にドメイン名やメアドなど等を設定し、`./setup.sh`を実行します。



## UNILORN's VPN DATA

## 参考サイト

- https://blog.ikappio.com/connect-macos-to-dockerized-l2tp-ipsec-server/
- https://ryuta46.com/1272

## Create VPN server

- EC2インスタンス作成
- セキュリティグループ、インバウンドルールの変更
    - UDP:500
    - UDP:4500

- Dockerのインストール
- docker-composeの実行

## Create User IKEv2

```bash
docker-compose exec l2tp-ipsec sh
sh ikev2.sh
[1]
<USER NAMEを入力>

生成された証明書を各自ダウンロードするなど

```

## VPN Client Setting

### Windows

- https://ryuta46.com/1272

### Android

- swann ファイルを端末にコピー
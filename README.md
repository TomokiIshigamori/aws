# AWS Web Server with Nginx

このプロジェクトは、AWS EC2上にNginxを使った簡単なWebサーバーを構築し、セキュリティ対策(Fail2ban、SSH設定強化)や自動バックアップなど、運用に役立つ構成を実装したものです。

##　特徴

- AWS EC2(Ubuntu 24.04)を使用
- Nginxで静的Webページをホスティング
- Fail2banで不正アクセスから保護
- SSHのセキュリティ強化済み
- バックアップスクリプトを実装
- GitHub Actionsを用いたデプロイ自動化

##　セットアップ方法

1. 本リポジトリをクローン
2. `.pem`ファイルを用いてSSH接続
3. `index.html`などを `/var/www/html` に配置
4. Nginx設定ファイルの編集と再起動
5. `backup.sh` スクリプトの実行権限を与えて定期実行

##　今後の予定

- ドメイン接続(Freenom)
- SSL化(Let's Encrypt予定)
- WordPressなど動的CMSへの応用

##　作者

[Tomoki Ishigamori](https://github.com/TomokiIshigamori)

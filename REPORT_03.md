# 第3回 Webエンジニアリング演習 レポート
## 学籍番号
4724116
## イメージとコンテナの違い
Dockerイメージはbuildでイメージを作り、実行に必要なものをまとめた読み取り専用のパッケージである。Dockerコンテナはrunでコンテナを作成・起動し、イメージから作られた実行中の環境である。
## Dockerfileの各行の役割
FROMは土台となるイメージを指定する。COPYはホストのファイルをイメージへコピーする。
## 動作確認
変更後の見出し　Docker Composeで配信中
docker compose psの結果　web-eng-docker-web-1   web-eng-docker-web   "/docker-entrypoint.…"   web       4 seconds ago   Up 3 seconds   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp

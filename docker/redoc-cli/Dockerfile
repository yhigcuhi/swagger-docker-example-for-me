# slim系のnodeから構築することを定義
FROM node:lts-bullseye

# コンテナ内の作業ディレクトリを作成
WORKDIR /var/www/html
# パッケージ一覧(インデックス)を更新
RUN apt update \
    && yarn install
# redoc cli導入
RUN npm install -g redoc-cli

# 公開ポート
EXPOSE 8080
# 起動時実行コマンド
ENTRYPOINT ["redoc-cli"]
CMD []

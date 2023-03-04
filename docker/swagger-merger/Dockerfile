# slim系のnodeから構築することを定義
FROM node:lts-bullseye

# コンテナ内の作業ディレクトリを作成
WORKDIR /var/www/html
# パッケージ一覧(インデックス)を更新
RUN apt update \
    && yarn install
# swagger-merger導入
RUN npm install -g swagger-merger watch
CMD ["swagger-merger"]

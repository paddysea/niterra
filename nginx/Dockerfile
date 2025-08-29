FROM nginx:alpine

# nginx設定ファイルをコピー
COPY nginx.conf /etc/nginx/nginx.conf
COPY conf.d/default.conf /etc/nginx/conf.d/default.conf

# 静的ファイルをnginxのhtmlにコピー
COPY ./public /var/www/html

# 適切な権限を設定
RUN chmod -R 755 /var/www/html
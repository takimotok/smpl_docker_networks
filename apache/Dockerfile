FROM httpd

COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf

# log 出力先 dir. 作成
RUN mkdir -p /tmp/logs/apache

EXPOSE 80

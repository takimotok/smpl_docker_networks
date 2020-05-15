FROM wordpress

# 日本語化
RUN apt-get update && apt-get -y upgrade \
  && apt-get -y install locales locales-all \
  && echo 'export LANG=ja_JP.UTF-8' >> ~/.bashrc \
  && echo 'export LANGUAGE="ja_JP:ja"' >> ~/.bashrc \
# vim が欲しい
  && apt-get -y install vim

ENV WORDPRESS_DB_HOST=mysql \
    WORDPRESS_DB_USER=root \
    WORDPRESS_DB_PASSWORD=docker01 \
    WORDPRESS_CONFIG_EXTRA="define('WP_HOME','http://localhost/blog/');define('WP_SITEURL','http://localhost/blog/');"


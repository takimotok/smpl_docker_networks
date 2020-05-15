FROM mysql:5.7

# 日本語化
RUN apt-get update && apt-get -y upgrade \
  && apt-get -y install locales locales-all \
  && echo 'export LANG=ja_JP.UTF-8' >> ~/.bashrc \
  && echo 'export LANGUAGE="ja_JP:ja"' >> ~/.bashrc \
  # vim が欲しい
  && apt-get -y install vim

ENV MYSQL_ROOT_PASSWORD=docker01

COPY ./mysql.cnf /etc/mysql/conf.d/mysql.cnf


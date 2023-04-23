FROM ubuntu:latest

LABEL maintainer="james@example.com"

ENV REFRESHED_AT 2023-23-04

RUN apt-get -qq update && apt-get -qq install nginx

RUN mkdir -p /var/www/html/website

ADD nginx/global.conf /etc/nginx/conf.d/

ADD nginx/nginx.conf /etc/nginx/

EXPOSE 80
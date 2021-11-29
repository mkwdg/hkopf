# Heroku-vless

## 概述
Heroku是一个支持多种编程语言的云平台即服务。目前支持Ruby、Java、Node.js、Scala、Clojure、Python、PHP和Perl等语言，基础操作系统是Debian。

本项目用于在 Heroku 上部署 vless+websocket+tls，每次部署自动选择最新的 alpine linux 和 xray core。相比vmess，vless的性能更加优秀，占用资源更少，运行更加稳定。

刚测试了一下，herokuapp.com这个域名已经被墙（2021.9.27），故现在如果不配置cf流量中转，这个将无法使用，建议使用cloudflare的workers的流量中转，速度更快，原则上不会有被墙风险。

## 镜像

经测试本镜像占用内存资源较低，运行稳定。

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://dashboard.heroku.com/new?template=https%3A%2F%2Fgithub.com%2Fmkwdg%2Fhkopf)

## 注意

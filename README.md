# オプティムチーム開発のための環境構築手順書

当リポジトリはオプティムメンバーの開発環境を統一するために作成したリポジトリである。

## 利用する条件
Docker,docker-compose,Gitをインストールしていること。

## 使用技術

言語 :golang 1.16.7  
Webアプリケーションフレームワーク :Gin  
webサーバ :Gin  
DBサーバ :mysql8.0

## 環境構築手順

step1 gin-practiceのリポジトリをcloneする。  
```
git clone https://github.com/jokertennis/gin-practice.git
```
step2 docker-imageを作成する。  
```
docker-compose build
```
step3 docker-containerを作成する。  
```
docker-compose up -d
```
step4 go_container,mysql_containerが立ち上がっていることを確認する。  
```
docker-compose ps
```
step5 hello,worldを確認する。  
```
curl http://localhost:8080/hello
```

## 主な参考文献

https://qiita.com/greenteabiscuit/items/ef4ed1dfda0d396d9d0f

## 文責

北見工業大学地域未来デザイン工学科地域マネジメント工学コース4年  
基盤コース：情報デザイン・コミュニケーション工学コース  
川田剣士(カワタケンジ)
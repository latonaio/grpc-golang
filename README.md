# grpc-golang
grpc-golang は、Golang で動作する(マイクロサービス)ランタイムにおける、gRPC の適用方法を記載したレポジトリです。  
Golangの場合、ライブラリの依存関係を共通レポジトリで構築できないため、AIONでは、Golangランタイムにおける gRPC の適用をマイクロサービス毎に定義しています。  

## 動作環境

* OS: Linux  
* CPU: ARM/AMD/Intel  
* Golang Runtime  

## Golang(マイクロサービス)ランタイム における grpc の適用方法  

Golang(マイクロサービスランタイム)環境で gRPC を適用する場合は、go.modに以下のように記載します。
```
module MODULE-NAME

go 1.17

require (
	google.golang.org/grpc v1.43.0-dev
	)
```
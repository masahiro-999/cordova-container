# cordova-container

Cordova, Node.js, Android sdkを含んだ開発環境を構築します
apkファイルのビルドまでできます

# 使い方

vscodeにRemote Developmentを入れ、Build and reopen in container開いれ使用してください

## プロジェクトの作成

```
$ $ cordova create hello-app
$ cd hello-app/
```

## ブラウザーで動作させる

```
$ cordova platform add browser
$ cordova run browser
```

## Android端末で動作させる
Android端末にUSB接続したadbで、adb tcpip 5555を実行しておく
Wifiで接続して、開発機と通信できる状態にする

```
$ cordova platform add android
$ adb connect 10.0.33.3:5555
$ cordova run android
```
10.0.33.3の部分はAndroid端末のWifi接続のIPアドレスに変更してください。
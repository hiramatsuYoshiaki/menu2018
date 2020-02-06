# vueapp0-cli3-scss

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

serve -s dist

ディプロイ（さくらインターネット）
tourdehdr.sakura.ne.jp/web3/vuecli3/
1.<base href="/">の追加
npm run build後に生成されたpublic/index.を編集
<!DOCTYPE html>
<html lang="jp">
  <head>
    <base href="/"> //＜－－－－－追加する
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <link rel="icon" href="<%= BASE_URL %>favicon.ico">
    <title>vueapp0-cli3-scss</title>
  </head>
  <body>
    <noscript>
      <strong>We're sorry but vueapp0-cli3-scss doesn't work properly without JavaScript enabled. Please enable it to continue.</strong>
    </noscript>
    <div id="app"></div>
  </body>
</html>
2.vue.config.jsの追加
プロジェクトルート（package.jsonのある階層）に、新しくvue.config.jsを作成し、下記を追加する。
module.exports = {
    baseUrl:'./web3/vuecli3/'
}
３．npm run buildを実行し、dist/index.htmlを確認する。
<!DOCTYPE html>
<html lang=en>
<head>
<base href=/ >　//<--追加
<meta charset=utf-8>
<meta http-equiv=X-UA-Compatible content="IE=edge">
<meta name=viewport content="width=device-width,initial-scale=1">
<link rel=icon href=web3/vuecli3/favicon.ico>　//<--追加　web3/vuecli3/
<title>vueapp0-cli3-scss</title>
<link href=web3/vuecli3/js/about.2d341050.js rel=prefetch>//<--追加　web3/vuecli3/
<link href=web3/vuecli3/css/app.c750f8b0.css rel=preload as=style>//<--追加　web3/vuecli3/
<link href=web3/vuecli3/js/app.d1faed55.js rel=preload as=script>//<--追加　web3/vuecli3/
<link href=web3/vuecli3/js/chunk-vendors.19368321.js rel=preload as=script>//<--追加　web3/vuecli3/
<link href=web3/vuecli3/css/app.c750f8b0.css rel=stylesheet>//<--追加　web3/vuecli3/
</head>
<body>
<noscript><strong>We're sorry but vueapp0-cli3-scss doesn't work properly without JavaScript enabled. Please enable it to continue.</strong></noscript>
<div id=app></div>
<script src=web3/vuecli3/js/chunk-vendors.19368321.js></script>//<--追加　web3/vuecli3/
<script src=web3/vuecli3/js/app.d1faed55.js></script>//<--追加　web3/vuecli3/
</body>
</html>

4.ftpでアップロードする。




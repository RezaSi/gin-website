---
sidebar:
  order: 1
title: まず始めに
---

Gin は Golang で書かれた Web アプリケーションフレームワークです。martini に似たAPIを持ちながら、httprouter
のおかげでそれより40倍以上も速いパフォーマンスがあります。良いパフォーマンスと生産性が必要であれば、Gin が好きになれるでしょう。

この章では、Gin とは何か、どんな問題を解決してくれるのか、そしてどのようにあなたのプロジェクトを助かるのかを説明します。

あなたがプロジェクトで Gin を使う準備がもし整っているのならば、[クイックスタート](../quickstart)を見てください。

## 機能

### 高速

基数木ベースのルーティング、そして小さなメモリ使用量。reflection は使っていません。予測可能なAPIパフォーマンス。

### ミドルウェアの支援

受け取った HTTP リクエストは、一連のミドルウェアと、最終的なアクションによって処理されます。 例：ログ出力、認証、GZIP
圧縮、そして最終的にDBにメッセージを投稿します。

### クラッシュフリー

Gin は、HTTP リクエストの処理中に発生した panic を recover
します。これにより、サーバーは常にユーザーからの応答を返すことができます。またこれにより例えば panic を Sentry
に送ったりすることも可能です！

### JSON バリデーション

Gin は JSON によるリクエストを解析してバリデーションすることができます。例えば必要な値の存在をチェックすることができます。

### ルーティングのグループ化

ルーティングをもっとよく整理しましょう。認証が必要かどうか、異なるバージョンのAPIかどうか...加えて、パフォーマンスを低下させることなく、無制限にネストしたグループ化を行うことができます。

### エラー管理

Ginは、HTTP
リクエスト中に発生したすべてのエラーを収集するための便利な方法を提供します。最終的に、ミドルウェアはそれらをログファイル、データベースに書き込み、ネットワーク経由で送信することができます。

### 組み込みのレンダリング

Ginは、JSON、XML、およびHTMLでレンダリングするための使いやすいAPIを提供します。

### 拡張性

とても簡単に新しいミドルウェアを作成できます。サンプルコードをチェックしてみてください。

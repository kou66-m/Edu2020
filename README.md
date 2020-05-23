# 全般

## Ruby, JavaScriptで共通する説明
Javaと比較して説明  
* 基本文法
    * Hello world?
    * コメント
    * リテラル (数値, 文字列, etc...)
    * データ型
* 変数, 定数宣言
* 演算子
* 制御構造
    * if
    * switch
    * while
    * for
    * 例外処理

キャメルケース, スネークケース


# JavaScript
https://developer.mozilla.org/ja/docs/Web/JavaScript

## 進め方
* ベースはテキスト
* 基礎構文、DOM操作、イベントの説明を適宜入れていく形
* 演習はテキストのプログラムに合わせて作る？
* JQueryの部分(6章)をピュアJSで行う？

## テキスト
基本構文, DOM操作 (HTMLに特化した部分), イベントが入り混じって説明されてる  
6章以降はJQuery、省略orJavaScriptで実装?

### 1章
* JavaScriptとは
* HTML, CSSの基礎

### 2章
* アウトプット周り (コンソール, アラート, 画面)

* 2-1
    * コンソールに出力
    * console.logの構文説明 <b><- ここにJavaとの比較を入れる? オブジェクト, フィールド, メソッド</b>
* 2-2
    * JSの記述場所 (CSSと同じイメージ)
    * コメント
* 2-3
    * window.alert
* 2-4
    * HTMLの書き換え (DOM操作)

### 3章
* 3-1
    * 条件分岐 (if)
    * true/false
* 3-2
    * 変数, 定数
    * var/let/constの違い
        * https://codezine.jp/article/detail/11353
        * https://qiita.com/39_isao/items/d9d80e98b5bd1938bc1d
    * 変数の巻き上げ  
    (varの場合はundefined, letの場合はReferenceErrorをスロー)
        * https://qiita.com/39_isao/items/d9d80e98b5bd1938bc1d
    * 比較演算子 (===)
* 3-3, 3-4
    * if, else if, ...
    * parseInt <- 組み込み関数
* 3-5
    * 論理演算子
* 3-6
    * while
    * 文字列連結 (数値+文字列も)
    * +=
* 3-7
    * 変数のスコープ
* 3-8
    * 関数定義
    * DOM操作
 * 3-9
    * FizzBuzz
    * 算術演算子
* 3-10
    * 配列
    * for .. of文
    * テンプレート文字列 (テンプレートリテラル)
    * insertAdjacentHTML
* 3-11
    * オブジェクト (連想配列)
    * for .. in文

### 4章
* 4-1
    * イベント（ハンドラ）
    * formのデータ読み取り (formの部品はname属性と同一のプロパティ値でアクセスできる？)
    * イベントのキャンセル
* 4-2
    * Dateオブジェクト
    * new構文
* 4-3
    * Mathオブジェクト

### 5章
* 5-1
    * setTimeout
* 5-2
    * location.href
    * document.querySelector
* 5-3
    * Cookie
    * <b>Web Serverが必要</b>
    * js-cookieライブラリを使用
* 5-4
    * data-*属性, datasetプロパティ
    * forEach
    * this
    * attrbuteへのアクセス

## 環境回り

### use strict;

### ESLint

* https://qiita.com/sifue/items/2b7687268661271039f5
* 


# Ruby
Ruby 2.6.x?

## 進め方
1. Java基礎編、オブジェクト指向編をまずRubyで置き換え
1. その後Ruby特有の書き方を説明？
    * イテレーションとかブロックとか
* 演習ベースで行うイメージ

# Rails
Rails 5.2.x?

## 環境
* WSL + Ubuntu?
* Slim使う?
* bootstrap (Gem install?)
* PostgreSQL

## テキスト

### 3章
CRUD (Without scaffold)

### 4章
* DB周り? (migration, model)
* ログイン, session  
-> has_secure_password (bcrypt Gem, パスワードのハッシュ化)
* ユーザ管理機能 (CRUD)
* Association (p170)
* ARのクエリメソッド (p176)
* controllerのfilter

### 5章
* テストツール

### 6章
* Routing
* タイムゾーン
* エラー処理
* ログ
* セキュリティ
* asset pipline

### 7章
* 検索機能の追加 (ransack Gem)  
-> Gemなしで作らせる?
* Action Mailer  
-> やらない?
* Active Storage
* CSV
* Pagenation (kaminari)
* 非同期処理

### 8章
* JavaScript
* Turbolinks

### 9章
* Git

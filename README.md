# README

## アプリケーション名
Pawnshop Manager

## アプリケーション概要
このアプリケーションは、質店の業務管理を目的としたアプリケーションです。
質入れ処理・利息管理・質返還処理・質流れ処理・買取処理・データ検索及び編集ができます。

## URL
https://github.com/grenade-Y-O-S/pawnshop_manager_35778

## 利用方法
BASIC認証を導入しています

ID:admin

pass:1234

## 目指した課題解決
質店は独特なシステムを用いて運営されており、扱う情報量が多いのでデータ管理をスムーズに行う事を目的として開発しました。

## 洗い出した要件
### 実装したい機能 / 要件(※背景色は、そのページの背景色と同じ色)
- トップページ

【ボタン】

・「入質」「利息」「買取」「質返還」「質流れ」「データ検索」のページへ遷移できるボタンがある

【表示】

・上記のボタンのみが表示される

- 入質ページ

【ボタン】

・新規客データを登録するページへ遷移できるボタンがある

・リピーター客のデータを検索するページへ遷移できるボタンがある

・トップページへ遷移できるボタンがある

【表示】

・上記のボタンのみが表示される

- 新規客データ登録ページ

【フォーム】
・入力項目
「姓」「名前」「姓(カタカナ)」「名前(カタカナ)」「住所」「電話番号」「生年月日」「職業」「備考」

【ボタン】
・新規客データを登録し、質データまたは買取データを登録するページへ遷移できるボタンがある
(遷移元が入質ページならば質データ登録ページへ、買取ページならば買取データ登録ページへ遷移する)

・入質ページへ遷移できるボタンがある

・トップページへ遷移できるボタンがある

- リピーター客データ検索ページ

【検索フォーム】

・検索項目をプルダウンで選択「客番号(客データID)」「姓(漢字)」「姓(カタカナ)」

・検索キーワードを入力

【ボタン】
・検索項目を選択し、質データまたは買取データを登録するページへ遷移できるボタンがある
(遷移元が入質ページならば質データ登録ページへ、買取ページならば買取データ登録ページへ遷移する)

・入質ページへ遷移できるボタンがある

・トップページへ遷移できるボタンがある

- 質データ登録ページ

【フォーム】

・入力項目

「品物名」「金額」「詳細」「備考」

【ボタン】

・質データを登録し、入力した客・質データを表示するページへ遷移できるボタンがある

・トップページへ遷移できるボタンがある

- 質登録データ表示ページ

【ボタン】

・トップページへ遷移できるボタンがある

【表示】
・登録した客データと質データを表示する

- 買取ページ

【ボタン】

・新規客データを登録するページへ遷移できるボタンがある
・リピーター客のデータを検索するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・上記のボタンのみが表示される

- 買取データ登録ページ

【フォーム】

・入力項目

「品物名」「金額」「詳細」

【ボタン】

・買取データを登録し、入力した客・買取データを表示するページへ遷移できるボタンがある

・トップページへ遷移できるボタンがある

- 買取登録データ表示ページ

【ボタン】
・トップページへ遷移できるボタンがある

【表示】
・登録した客データと買取データを表示する

- 利息検索ページ

【検索フォーム】
・検索項目をプルダウンで選択
「客番号(客データID)」「姓(漢字)」「姓(カタカナ)」
・検索キーワードを入力
・利息データを紐づける質データを検索する

【ボタン】
・検索結果を表示するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 利息検索結果表示ページ

【ボタン】
・表示された質データの中から、利息データと紐づけるものを選択し、利息データ入力ページへ遷移できるボタンがある
・質データを検索するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・検索した質データが一覧表示される

- 利息データ登録ページ

【フォーム】
・入力項目
「利息回数」

【ボタン】
・利息データを登録し、入力した利息データと紐づけた質データを表示するページへ遷移できるボタンがある
・質データを検索するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・紐づけた質データを表示する

- 利息登録データ表示ページ

【ボタン】
・登録した利息データと、それにより変化した質の期限を表示するページへ遷移できるボタンがある
・質データを検索するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・登録した利息データと、紐づけた質データが表示される
「質番号(質データID)」「客氏名(姓+名前)」「金額」「利息金額」「備考」「入質日」「これまでの利息合計」「期限」

- 質返還/質流れ検索ページ

【検索フォーム】
・検索項目をプルダウンで選択
「質番号(質データID)」「姓(漢字)」「姓(カタカナ)」
・検索キーワードを入力
・情報を変更する質データを検索する

【ボタン】
・検索結果を表示するページへ遷移できるボタンがある
(遷移元が質返還ボタンならば「返還済み」に、質流れボタンならば「質流れ」に状態を変更する。質流れに変更する時は背景色はグレー)
・トップページへ遷移できるボタンがある

- 質返還/質流れ検索結果表示ページ
【ボタン】
・表示された質データの中から、状態を変更するものを選択し、変更処理を行うページへ遷移できるボタンがある
・質データを検索するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・検索した質データが一覧表示される

- 質返還/質流れ変更処理ページ

【ボタン】
・質データの状態を変更し、変更結果を表示するページへ遷移できるボタンがある
・質データを検索するページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・選択した質データと、それに紐づく客データが表示される

- 質返還/質流れ変更結果表示ページ

【ボタン】
・トップページへ遷移できるボタンがある

【表示】
・変更した質データと、それに紐づく客データが表示される

- データ検索ページ

【ボタン】
・客データ検索ページへ遷移できるボタンがある
・質データ検索ページへ遷移できるボタンがある
・利息データ検索ページへ遷移できるボタンがある
・買取データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・上記のボタンのみが表示される

- 客データ検索ページ

【検索フォーム】
・検索項目をプルダウンで選択
「客番号(客データID)」「姓(漢字)」「姓(カタカナ)」
・検索キーワードを入力

【ボタン】
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 客データ検索結果一覧ページ

【ボタン】
・客データを選択し、客データ編集ページへ遷移できるボタンがある
・客データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・客データの検索結果一覧およびデータ編集ボタンが表示される

- 客データ編集ページ

【編集フォーム】
・客データの全項目を入力する

【ボタン】
・客データを編集し、その客データを表示するページへ遷移できるボタンがある
・客データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

客データ編集結果表示ページ
【ボタン】
・トップページへ遷移できるボタンがある

【表示】
・編集した客データが表示される

- 質データ検索ページ

【検索フォーム】
・検索項目をプルダウンで選択
「質番号(質データID)」「姓(漢字)」「姓(カタカナ)」
・検索キーワードを入力

【ボタン】
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 質データ検索結果一覧ページ

【ボタン】

・質データを選択し、質データ編集ページへ遷移できるボタンがある
・質データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・質データの検索結果一覧およびデータ編集ボタンが表示される

- 質データ編集ページ

【編集フォーム】
・質データの全項目を入力する

【ボタン】
・質データを編集し、その質データを表示するページへ遷移できるボタンがある
・質データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 質データ編集結果表示ページ
【ボタン】
・トップページへ遷移できるボタンがある

【表示】
・編集した質データが表示される

- 買取データ検索ページ
【検索フォーム】
・検索項目をプルダウンで選択
「買取番号(買取データID)」「姓(漢字)」「姓(カタカナ)」
・検索キーワードを入力

【ボタン】
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 買取データ検索結果一覧ページ

【ボタン】
・買取データを選択し、買取データ編集ページへ遷移できるボタンがある
・買取データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・買取データの検索結果一覧およびデータ編集ボタンが表示される

- 買取データ編集ページ

【編集フォーム】
・買取データの全項目を入力する

【ボタン】
・買取データを編集し、その買取データを表示するページへ遷移できるボタンがある
・買取データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 買取データ編集結果表示ページ

【ボタン】
・トップページへ遷移できるボタンがある

【表示】
・編集した買取データが表示される

- 利息データ検索ページ

【検索フォーム】
・検索項目をプルダウンで選択
「利息番号(利息データID)」「質番号(質データID)」「姓(漢字)」「姓(カタカナ)」
・検索キーワードを入力

【ボタン】
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 利息データ検索結果一覧ページ

【ボタン】
・利息データを選択し、利息データ編集ページへ遷移できるボタンがある
・利息データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

【表示】
・利息データの検索結果一覧およびデータ編集ボタンが表示される

- 利息データ編集ページ

【編集フォーム】
・利息データを入力する

【ボタン】
・利息データを編集し、その利息データとそれに紐づく質データを表示するページへ遷移できるボタンがある
・利息データ検索ページへ遷移できるボタンがある
・データ検索ページへ遷移できるボタンがある
・トップページへ遷移できるボタンがある

- 利息データ編集結果表示ページ

【ボタン】
・トップページへ遷移できるボタンがある

【表示】
・編集した利息データと、それに紐づく質データが表示される

## 実装した機能についての画像やGIFおよびその説明
[![Image from Gyazo](https://i.gyazo.com/1502b96c2e1f5fcf1f21f70938481966.gif)](https://gyazo.com/1502b96c2e1f5fcf1f21f70938481966)

[![Image from Gyazo](https://i.gyazo.com/da81c47d8371568dfca611795f6f225b.gif)](https://gyazo.com/da81c47d8371568dfca611795f6f225b)
まず客データを登録し、それに紐づく質データを登録する(どのページでも確認のポップアップが出る)

[![Image from Gyazo](https://i.gyazo.com/2f039dc7270a118f5898f1a0f37f5b1f.gif)](https://gyazo.com/2f039dc7270a118f5898f1a0f37f5b1f)

[![Image from Gyazo](https://i.gyazo.com/1f1f14858e2080fd3e25e4162ed37d9c.gif)](https://gyazo.com/1f1f14858e2080fd3e25e4162ed37d9c)

[![Image from Gyazo](https://i.gyazo.com/50868e317d928ab5954f837b51e30a70.gif)](https://gyazo.com/50868e317d928ab5954f837b51e30a70)
すでにデータがある客については検索から質データに紐付ける事ができる
(買取も同じ手順)

[![Image from Gyazo](https://i.gyazo.com/4ed691e173c9e61e5ff7fd3935361fd9.gif)](https://gyazo.com/4ed691e173c9e61e5ff7fd3935361fd9)

[![Image from Gyazo](https://i.gyazo.com/123077445b6f9f21b35f686131bf73bc.gif)](https://gyazo.com/123077445b6f9f21b35f686131bf73bc)
質データを検索し、その質データに紐づく利息データを登録する。登録後は、更新された期限等が表示される

[![Image from Gyazo](https://i.gyazo.com/9b15ef86bb1ddb614d8d672fc555e14b.png)](https://gyazo.com/9b15ef86bb1ddb614d8d672fc555e14b)
データ検索ページにて、質データを検索した画面
客の氏名、質の貸付金額、利息金額、これまで支払った利息の回数、期限を表示している

[![Image from Gyazo](https://i.gyazo.com/24ef8d2086f4ff0df349e52647c94bed.gif)](https://gyazo.com/24ef8d2086f4ff0df349e52647c94bed)

[![Image from Gyazo](https://i.gyazo.com/8ffef207a0dee320b1e7a588ae07fbe2.gif)](https://gyazo.com/8ffef207a0dee320b1e7a588ae07fbe2)
質返還処理。取引状態を返還済に変更する(重要な手順なので独立させている)

[![Image from Gyazo](https://i.gyazo.com/14147ccfc9f458571c296298ae9c97de.gif)](https://gyazo.com/14147ccfc9f458571c296298ae9c97de)

[![Image from Gyazo](https://i.gyazo.com/85540234fa637ebc1a2031ecd1320323.gif)](https://gyazo.com/85540234fa637ebc1a2031ecd1320323)
質流れ処理。取引状態を質流れに変更する。

[![Image from Gyazo](https://i.gyazo.com/dc0f3ca5db07a0218ccb4131b958211f.png)](https://gyazo.com/dc0f3ca5db07a0218ccb4131b958211f)
質データ検索結果ページにて、質データが返還済である事が黄色背景・黒文字で表示されている

[![Image from Gyazo](https://i.gyazo.com/47ba40a283683adc30532942ab29063a.png)](https://gyazo.com/47ba40a283683adc30532942ab29063a)
同じく、質データが質流れである事が白背景・黒文字で表示されている


## 実装予定の機能
- データ検索で、検索条件に日付を指定できるようにする

- データ検索で、複数の検索条件で検索できるようにする

- 利息データ登録画面で、入力した利息回数に応じて支払う利息金額を表示されるようにする

- 新規の客データを登録する時、生年月日から客の年齢を算出し、18歳未満ならば警告が出るようにする(18歳未満が質取引を利用する事は違法)

- 毎日19時以降になると、その日1日の業務内容を確認するページのリンクをトップページに表示する

- 金やプラチナの相場データを登録し、質や買取の登録ページに相場データ表示ページへのリンクを表示する

## データベース設計
![ER](lib/img/er.png)

## customersテーブル

| Column          | Type   | Options     |
|-----------------|--------|-------------|
| last_name       | string | null: false |
| first_name      | string | null: false |
| last_name_kana  | string | null: false |
| first_name_kana | string | null: false |
| address         | string | null: false |
| phone_number    | string | null: false |
| birth_date      | date   | null: false |
| job             | string | null: false |
| remarks         | text   |             |


### Association
-  has_many :pawns
-  has_many :purchases


## pawnsテーブル

| Column       | Type       | Options                        |
|--------------|------------|--------------------------------|
| item_name    | string     | null: false                    |
| item_price   | integer    | null: false                    |
| item_detail  | text       | null: false                    |
| item_remarks | text       |                                |
| item_status  | integer    | null: false                    |
| customer     | references | null: false, foreign_key: true |

### Association
-  belongs_to :customer
-  has_many   :interests


## interestsテーブル

| Column           | Type       | Options                        |
|------------------|------------|--------------------------------|
| interests_number | integer    | null: false                    |
| pawn             | references | null: false, foreign_key: true |

### Association
-  belongs_to :pawn


## purchasesテーブル

| Column          | Type       | Options                        |
|-----------------|------------|--------------------------------|
| buy_item_name   | string     | null: false                    |
| buy_item_price  | integer    | null: false                    |
| buy_item_detail | text       | null: false                    |
| customer        | references | null: false, foreign_key: true |

### Association
-  belongs_to :customer

## ローカルでの動作方法

1.GitHubの、このアプリケーションのページを開く (https://github.com/grenade-Y-O-S/pawnshop_manager_35778)
2.画面右上にある「Clone or dowload」ボタンをクリックするとURLがクリップボードにコピーされる
3.コマンドプロンプトに「$ git clone クリップボードにコピーしたURL」と入力する
4.レポジトリ名のフォルダができ、その中にファイルがダウンロードされる
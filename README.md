# 職務経歴

本名や会社名、製品名は伏せています。

## 基本情報

- name: fourside
- github: https://github.com/fourside

## 資格

| 取得年月 | 資格                        |
| :------: |-----------------------------|
| 2002/11  | TOEIC 700                   |
| 2009/11  | 基本情報技術者              |
| 2010/09  | LPIC-1                      |
| 2010/12  | 応用情報技術者              |
| 2017/08  | Java Programmer, Silver SE8 |
| 2017/10  | Java Programmer, Gold SE8   |

## 職務経歴

| from     | to        | 会社名           |
|:--------:|:---------:|------------------|
| 2020/05  | 現在      | フリーランス     |
| 2019/12  | 2020/04   | 株式会社 A(仮)   |
| 2018/04  | 2019/09   | 株式会社 B(仮)   |
| 2011/01  | 2018/03   | 株式会社 C(仮)   |

## 職務内容

### フリーランスでの案件について

#### アプリケーション内のサブシステム構築
- 期間: 2ヶ月
- 言語: JavaScript(Node.js)
- 内容
    - VPC内で使用されるWebAPIの作成
        - ElastiCache(Redis) - Lambda - API Gateway
    - RDB/Redisを更新するバッチ処理
        - CloudWatch Event(schedule) - Lambda - RDS(mysql)/ElastiCache(Redis)
        - RDS の更新後にRedisの更新を行う連携にSQSを使った
    - 上記AWSリソースをCloudFormationで構築
    - テストを書きながら実装することができた

#### WebScokectを使ったWebアプリケーションの引き継ぎ
- 期間: 2週間
- 言語: TypeScript
- ライブラリ
    - Angular9
    - socket.io
    - Express
- 内容
    - 前任者が期限中に終えられなかった案件を引き継いた
        - できていたのはWebSocketの連携部分のみで、ローカル起動できない状態だった
    - やったこと
        - 3Dアニメーションの実装(6面体、12面体、18面体)
        - レイアウト修正
        - WebSocket再接続処理
        - バックエンドとフロントエンドの分離
        - インフラ構築が面倒だったので Docker にアプリを押し込めてリリースした

### 株式会社 A(仮)
- サーバレスで CtoC サービスの開発
- 言語: JavaScript(Node.js), TypeScript(browser)
- ライブラリ/使用しているサービス: React(CRA), aws-amplify
- 担当: 設計、実装
    - stripeを使った決済処理
    - JSからTSへの移行
    - パフォーマンスのチューニングなど
        - 頻繁にアクセスするデータをContextに持たせる
        - アップロードされた画像をそのまま表示せず加工する
    - アプリとslackの連携処理
    - その他リファクタリング
        - なるべくロジックをコンポーネントから剥がしたり、メール本文をテンプレート(mustache)を使ったりした

### 株式会社 B(仮)
- パッケージ開発、クラウドサービスの開発
- 言語: Java
- 担当: 設計、実装
- その他、Java8からJava11への移行調査など

### 株式会社 C(仮)
- SESだったため期間ごとに記載します

| from     | to        | 業務内容 |
|:--------:|:---------:|----------|
| 2011/01  | 2011/11   | 物流システムの統合 |
| 2012/01  | 2014/03   | 非接触型 IC カードと連携する Web システム開発と保守 |
| 2014/04  | 2018/03   | パッケージ製品間の通信をインターネットで行うWebサービス開発 |

#### パッケージ製品間の通信をインターネットで行うWebサービス開発

- 概要: WebSocketで製品間の通信をラップするWebサービスの開発
- 言語: Java, JavaScript
- ミドルウェア: postgres, wildfly, nginx, apache
- 担当: 設計、実装、運用
- やったこと
    - 主に管理画面
        - サーバサイドはREST API
        - フロントエンドは AngularJSでSPA
        - その他にも「コードは共同所有」の方針でだいたいのものに自分の手が入ってる
    - アジャイル開発
        - 2週間を1イテレーションとしてユーザーストーリーを消化していく
        - Jenkins
            - ビルド -> デプロイ -> 受入テスト
    - AWS上に環境を構築
        - 使用した主なサービス: ec2, rds, cloudwatch, sns, ses
        - 構築当初は社内プロクシを超え、多段sshする設定に苦労した
    - バンドルしていなかったJavaScriptをビルドするようにした
        - ついでにlintやunit testを回すようにした
    - 運用につらさを感じてansible/flywayを導入した

#### 非接触型 IC カードと連携する Web システム開発と保守

- 概要: 来店したユーザに対しクーポンを配布するWebシステムの開発
- 言語: PHP
- ミドルウェア: apache, mysql
- 担当: 設計、実装、保守運用
- やったこと
    - マイページ機能の追加
    - バッチの改善
        - 実行時間1hから2,3minに短縮
    - 保守作業として月次の脆弱性調査
    - キャンペーンサイトをスクラッチで作成
        - フレームワークを使わない縛りがあった

#### 物流システムの統合

- 概要: EDIのデータを内部データ形式に変換し、帳票を作成
- 言語: COBOL
- 担当: 実装、単体テスト

## スキル

### 現在よく使っているもの
- JavaScript
    - React 16
    - Node.js
    - webpack
- TypeScript
- HTML/CSS
- docker/docker-compose
- AWS
    - ec2/s3/lambda/cloudwatch/rds/ses/sns/sqs/amplify/cdk/cloudformation/dynamodb/api gateway
- Vim

### 昔触っていたもの
- JavaScript
    - AngularJS 1.2/Angular 4
    - gulp
- Java
    - SE8
    - JavaEE 7
- PHP 5.6
    - ZendFramework/Smarty/Doctrine
- Ruby 2.1
    - Ruby on Rails 2.x / Sinatra 1.3
- Apache/nginx
- misc
    - ansible
    - flyway
    - Jenkins
    - selenium

## つよみ
- つよみらしいことを書けないので[自己紹介ブログ](https://fourside.github.io/about-me)を書きました。

## よわみ
- 朝

## 興味のあること

### React Native
- スマホアプリを作るにはハードルがあったので試してみたい

## 参考
- [職務経歴書をGitHubで管理しよう - Qiita](https://qiita.com/okoysm/items/abcad0b4aefa585bc50b)
- [職務経歴書をGitHubに公開するのはいいぞ #職務経歴書 - 空飛ぶ羊](http://okoysm.hatenablog.jp/entry/2016/12/19/060000)


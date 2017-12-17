# 職務経歴

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
| 2011/01  | 現在      | 株式会社 xxx(仮) |

## 職務内容

### 株式会社 xxx(仮)

| from     | to        | 業務内容 |
|:--------:|:---------:|----------|
| 2011/01  | 2011/11   | 物流システムの統合 |
| 2012/01  | 2014/03   | 非接触型 IC カードと連携する Web システム開発と保守 |
| 2014/04  | 現在      | パッケージ製品間の通信をインターネットで行うWebサービス開発 |

#### パッケージ製品間の通信をインターネットで行うWebサービス開発

- 概要: WebSocketで製品間の通信をラップするWebサービスの開発
- 使用言語: Java, JavaScript
- 担当: 設計、実装、運用
- やったこと
    - 主に管理画面(サーバサイド、フロントエンド)
    - アジャイル開発
        - JenkinsでCIを回す
            - ビルドごとにJUnitで作った受け入れテストを実行
    - AWS上に環境を構築
        - 使用した主なサービス: ec2, rds, cloudwatch, sns, ses
        - 構築当初は社内プロクシを超え、多段sshする設定に苦労した
    - バンドルしていなかったJavaScriptをビルドするようにした
        - ついでにlintやunit testを回すようにした
    - 運用につらさを感じてansible/flywayを導入した

#### 非接触型 IC カードと連携する Web システム開発と保守

- 概要: 来店したユーザに対しクーポンを配布するWebシステムの開発
- 使用言語: PHP
- 担当: 設計、実装、保守運用
- やったこと
    - バッチの改善
        - 実行時間1hから2,3minに短縮
    - 保守作業として月次の脆弱性調査

#### 物流システムの統合

- 概要: EDIのデータを内部データ形式に変換し、帳票を作成
- 使用言語: COBOL
- 担当: 実装、単体テスト

## スキル
- Java
    - SE8
    - JavaEE 7
        - JAX-RS(resteasy)
        - WebSocket(undertow)
        - JPA(hibernate)
- JavaScript
    - AngularJS 1.2/Angular 4
    - TypeScript 2.0
- HTML5/CSS3
    - Bootstrap 3.3
- PHP 5.6
    - ZendFramework/Smarty/Doctrine
- Ruby 2.1
    - Ruby on Rails 2.1 / Sinatra 1.3
- Vim 8
- Apache/nginx
- tool
    - ansible
    - flyway
    - Jenkins
    - selenium

## つよみ

## よわみ
- 朝
- 自己評価が低い(らしい)

## やったことがないが興味のあること

### 関数型言語
知らない概念を得たい。Haskelを勉強したい。

### IoT
電子工作でも。技術を暮らしに活かしたい。

### クラウド
やってるけど、クラウドらしい使い方はできていない。


## 参考
- [職務経歴書をGitHubで管理しよう - Qiita](https://qiita.com/okoysm/items/abcad0b4aefa585bc50b)
- [職務経歴書をGitHubに公開するのはいいぞ #職務経歴書 - 空飛ぶ羊](http://okoysm.hatenablog.jp/entry/2016/12/19/060000)


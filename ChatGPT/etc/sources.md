# プロジェクトで使用するデータの情報源

本ファイルは、本プロジェクトに提供されるデータの出典と、各 Dropbox フォルダの役割を定義する。

- フォルダ名およびファイル名は、原則としてコード表記する。
- 以下に用途が記載されていないフォルダやファイルについては、名称だけから内容を推測しない。

## Dropbox フォルダ

### 共通

- 各フォルダ内のファイルの概要は各フォルダ直下にある `README.md` を参照する。
- `README.md` にないものは ChatGPT が推測して判断する。

### 小説作品

- フォルダ `Dropbox\scribe\novel` 以下の正規表現 `/^(?<op>op\d+)$/` にマッチするフォルダは、長編小説作品を収録する。
  - 名前付きキャプチャグループ `op` は、`op65` のような作品識別子全体を取得する。
- `opss` は、短編小説作品をまとめたフォルダで正規表現 `/^(?<op>ssop\d+)$/` にマッチするフォルダは、個別の作品を収録する。
  - 名前付きキャプチャグループ `op` は、`ssop008` のような作品識別子全体を取得する。

### 小説関連

| フォルダ名 | 内容 |
|---|---|
| `Dropbox\scribe\novel\story-world` | 小説作品の世界設定 |
| `Dropbox\scribe\project\novel-creating-method` | 小説の制作手法 |
| `Dropbox\scribe\novel\novel-etc` | 小説に関するその他の情報 |
| `Dropbox\scribe\project\research-of-literary-ornamentation` | 文彩の研究 |
| `Dropbox\scribe\project\research-of-narrative-construction` | 物語構築の研究 |
| `Dropbox\scribe\project\research-of-novel-creation` | 小説制作の研究 |
| `Dropbox\scribe\project\research-of-world-building` | 世界設定の研究 |
| `Dropbox\www\satsuki.c` | 小説制作サポートサイト |

### その他

| フォルダ名 | 内容 |
|---|---|
| `Dropbox\ai` | AI の運用に関するデータ |
| `Dropbox\external-relations\等身大の点と点委員会` | 等身大の点と点委員会に関するデータ |
| `Dropbox\www\studio\common` | 複数の用途で共有するデータ |
| `Dropbox\www\satsuki` | 公式ホームページのデータ |
| `Dropbox` | 日常生活の管理 |
| `Dropbox\www\studio\etc` | JavaScript などの小品 |

### ライブラリ

| フォルダ名 | 内容 |
|---|---|
| `Dropbox\www\studio\brackettool.js` | 文書内の括弧を処理する JavaScript ライブラリ |
| `Dropbox\www\studio\comparearray.js` | 配列を比較する JavaScript ライブラリ |
| `Dropbox\www\studio\htmlshape.js` | HTML を整形する JavaScript ライブラリ |
| `Dropbox\www\studio\maketable.js` | 配列からテーブルを生成する JavaScript ライブラリ |
| `Dropbox\www\studio\mdparse.js` | Markdown を HTML に変換する JavaScript ライブラリ |
| `Dropbox\www\studio\notion-customization` | ユーザー CSS によって Notion の Web サイトをカスタマイズするためのデータ |
| `Dropbox\www\studio\novelparse.js` | Web 小説の文書を HTML に変換する JavaScript ライブラリ |
| `Dropbox\www\studio\replacetool.js` | 文字列の置換処理を行う JavaScript ライブラリ |
| `Dropbox\www\studio\textodt.js` | テキストファイルを ODT 形式に変換する JavaScript ライブラリ |
| `Dropbox\www\studio\wordcount.js` | 文字数を数える JavaScript ライブラリ |
| `Dropbox\www\studio\yamlparse.js` | YAML を Web 上で読みやすく表示する JavaScript ライブラリ |

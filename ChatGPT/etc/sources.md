# プロジェクトで使用するデータの情報源

本ファイルは、本プロジェクトに提供されるデータの出典と、各 GitHub リポジトリの役割を定義する。

- リポジトリ名およびファイル名は、原則としてコード表記する。
- 以下に用途が記載されていないリポジトリやファイルについては、名称だけから内容を推測しない。

## GitHub リポジトリ

### 小説作品

- 正規表現 `/^(?<op>op\d+)$/` にマッチするリポジトリは、長編小説作品を収録する。
  - 名前付きキャプチャグループ `op` は、`op72` のような作品識別子全体を取得する。
- `ssop` は、短編小説作品をまとめたリポジトリである。

### 小説関連

| リポジトリ名 | 内容 |
|---|---|
| `story-world` | 小説作品の世界設定 |
| `novel-creating-method` | 小説の制作手法 |
| `novel-etc` | 小説に関するその他の情報 |
| `research-of-literary-ornamentation` | 文彩の研究 |
| `research-of-narrative-construction` | 物語構築の研究 |
| `research-of-novel-creation` | 小説制作の研究 |
| `research-of-world-building` | 世界設定の研究 |
| `satsuki.c` | 小説制作サポートサイト |

### その他

| リポジトリ名 | 内容 |
|---|---|
| `ai` | AI の運用に関するデータ |
| `life-sized-dot-to-dot-committee` | 等身大の点と点委員会に関するデータ |
| `common` | 複数の用途で共有するデータ |
| `satsuki` | 公式ホームページのデータ |
| `top-folder` | 日常生活の管理 |
| `etc` | JavaScript などの小品 |

### ライブラリ

| リポジトリ名 | 内容 |
|---|---|
| `brackettool.js` | 文書内の括弧を処理する JavaScript ライブラリ |
| `comparearray.js` | 配列を比較する JavaScript ライブラリ |
| `htmlshape.js` | HTML を整形する JavaScript ライブラリ |
| `maketable.js` | 配列からテーブルを生成する JavaScript ライブラリ |
| `mdparse.js` | Markdown を HTML に変換する JavaScript ライブラリ |
| `notion-customization` | ユーザー CSS によって Notion の Web サイトをカスタマイズするためのデータ |
| `novelparse.js` | Web 小説の文書を HTML に変換する JavaScript ライブラリ |
| `replacetool.js` | 文字列の置換処理を行う JavaScript ライブラリ |
| `textodt.js` | テキストファイルを ODT 形式に変換する JavaScript ライブラリ |
| `wordcount.js` | 文字数を数える JavaScript ライブラリ |
| `yamlparse.js` | YAML を Web 上で読みやすく表示する JavaScript ライブラリ |

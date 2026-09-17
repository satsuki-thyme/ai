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
- フォルダ `Dropbox\scribe\novel\opss` は短編小説作品をまとめたもので、それ以下にあるフォルダで正規表現 `/^(?<op>ssop\d+)$/` にマッチするものは個別の作品を収録する。
  - 名前付きキャプチャグループ `op` は、`ssop008` のような作品識別子全体を取得する。

### 小説関連

| フォルダ名 | 内容 |
|---|---|
| `Dropbox\scribe\novel\novel-etc` | 小説に関するその他の情報 |
| `Dropbox\scribe\novel\story-world` | 小説作品の世界設定 |
| `Dropbox\scribe\project\novel-creating-method` | 小説の制作手法 |
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

## GitHub リポジトリの対応

- この節のリポジトリはすべて GitHub アカウント `satsuki-thyme` のものとする。
- この対応は GitHub API で反映先候補を特定するために使う。更新前には、リポジトリの存在、書き込み権限、対象ブランチ、更新対象ファイルの対応を確認する。
- 表にない Dropbox フォルダ、または表の規則だけでリポジトリ内のファイルパスを確認できない場合は、推測で GitHub に変更を加えない。

### ルート対応

| Dropbox フォルダ | GitHub リポジトリ | パスの対応 |
|---|---|---|
| `Dropbox\ai` | `satsuki-thyme/ai` | `Dropbox\ai\` より後の相対パスを、区切りを `/` にしてリポジトリ内パスにする。 |

### 小説作品

| Dropbox フォルダまたはパターン | GitHub リポジトリ |
|---|---|
| `Dropbox\scribe\novel\opNN` | `satsuki-thyme/opNN` |
| `Dropbox\scribe\novel\opss\ssopNN` | `satsuki-thyme/opss` |
| `Dropbox\scribe\novel\novel-etc` | `satsuki-thyme/novel-etc` |
| `Dropbox\scribe\novel\story-world` | `satsuki-thyme/story-world` |
| `Dropbox\scribe\project\novel-creating-method` | `satsuki-thyme/novel-creating-method` |
| `Dropbox\scribe\project\research-of-literary-ornamentation` | `satsuki-thyme/research-of-literary-ornamentation` |
| `Dropbox\scribe\project\research-of-narrative-construction` | `satsuki-thyme/research-of-narrative-construction` |
| `Dropbox\scribe\project\research-of-novel-creation` | `satsuki-thyme/research-of-novel-creation` |
| `Dropbox\scribe\project\research-of-world-building` | `satsuki-thyme/research-of-world-building` |
| `Dropbox\www\satsuki.c` | `satsuki-thyme/satsuki.c` |

### その他

| Dropbox フォルダ | GitHub リポジトリ |
|---|---|
| `Dropbox\external-relations\等身大の点と点委員会` | `satsuki-thyme/life-sized-dot-to-dot-committee` |
| `Dropbox\www\studio\common` | `satsuki-thyme/common` |
| `Dropbox\www\satsuki` | `satsuki-thyme/satsuki` |
| `Dropbox\www\studio\etc` | `satsuki-thyme/etc` |

### ライブラリ

| Dropbox フォルダまたはファイル | GitHub リポジトリ |
|---|---|
| `Dropbox\www\studio\brackettool.js` | `satsuki-thyme/brackettool.js` |
| `Dropbox\www\studio\comparearray.js` | `satsuki-thyme/comparearray.js` |
| `Dropbox\www\studio\htmlshape.js` | `satsuki-thyme/htmlshape.js` |
| `Dropbox\www\studio\maketable.js` | `satsuki-thyme/maketable.js` |
| `Dropbox\www\studio\mdparse.js` | `satsuki-thyme/mdparse.js` |
| `Dropbox\www\studio\notion-customization` | `satsuki-thyme/notion-customization` |
| `Dropbox\www\studio\novelparse.js` | `satsuki-thyme/novelparse.js` |
| `Dropbox\www\studio\replacetool.js` | `satsuki-thyme/replacetool.js` |
| `Dropbox\www\studio\textodt.js` | `satsuki-thyme/textodt.js` |
| `Dropbox\www\studio\wordcount.js` | `satsuki-thyme/wordcount.js` |
| `Dropbox\www\studio\yamlparse.js` | `satsuki-thyme/yamlparse.js` |


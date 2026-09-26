# プロジェクトで使用するデータの情報源

本ファイルは、本プロジェクトに提供されるデータの出典と、各 Dropbox フォルダの役割を定義する。

- フォルダ名およびファイル名は、原則としてコード表記する。
- 以下に用途が記載されていないフォルダやファイルについては、名称だけから内容を推測しない。

## Dropbox フォルダ

### 共通

- 各フォルダ内のファイルの概要は各フォルダ直下にある `README.md` を参照する。
- `README.md` にないものは AI が推測して判断する。

### 小説作品

- フォルダ `Dropbox\scribe\novel` 以下の正規表現 `/^(?<op>op\d+)$/` にマッチするフォルダは、長編小説作品を収録する。
  - 名前付きキャプチャグループ `op` は、`op65` のような作品識別子全体を取得する。
- フォルダ `Dropbox\scribe\novel\ss` は短編小説作品をまとめたもので、それ以下にあるフォルダで正規表現 `/^(?<op>ssop\d+)$/` にマッチするものは個別の作品を収録する。
  - 名前付きキャプチャグループ `op` は、`ssop008` のような作品識別子全体を取得する。

### 小説制作関連

| Dropbox フォルダまたはパターン | 内容 | GitHub リポジトリ |
|---|---|---|
| `Dropbox\scribe\novel\opNN` | 長編小説作品群 | `satsuki-thyme/opNN` |
| `Dropbox\scribe\novel\ss\ssopNN` | ショートストーリー作品群 | `satsuki-thyme/ss` |
| `Dropbox\scribe\novel\novel-etc` | 小説に関するその他の情報 | `satsuki-thyme/novel-etc` |
| `Dropbox\scribe\novel\story-world` | 小説作品の世界設定 | `satsuki-thyme/story-world` |
| `Dropbox\www\satsuki.c` | 小説制作サポートサイト | `satsuki-thyme/satsuki.c` |

### 小説学習・研究

| Dropbox フォルダまたはパターン | 内容 | GitHub リポジトリ |
|---|---|---|
| `Dropbox\scribe\project\novel-creating-method` | 小説の制作手法 | `satsuki-thyme/novel-creating-method` |
| `Dropbox\scribe\project\research-of-literary-ornamentation` | 文彩の研究 | `satsuki-thyme/research-of-literary-ornamentation` |
| `Dropbox\scribe\project\research-of-narrative-construction` | 物語構築の研究 | `satsuki-thyme/research-of-narrative-construction` |
| `Dropbox\scribe\project\research-of-novel-creation` | 小説制作の研究 | `satsuki-thyme/research-of-novel-creation` |
| `Dropbox\scribe\project\research-of-world-building` | 世界設定の研究 | `satsuki-thyme/research-of-world-building` |

### コンピュータ機能開発

| Dropbox フォルダまたはパターン | 内容 | GitHub リポジトリ |
|---|---|---|
| `Dropbox\www\studio\character-relationship-chart` | キャラクター相関図 | `satsuki-thyme/character-relationship-chart` |
| `Dropbox\www\studio\KALA-Timer` | KALA Timer | `satsuki-thyme/KALA-Timer` |
| `Dropbox\www\studio\quick-highlight` | ハイライトのVS Code拡張機能 | なし |
| `Dropbox\scribe\project\novel-creator` | 小説クリエイター（ChatGPTプロジェクト） | `satsuki-thyme/novel-creator` |

### ルート対応

| Dropbox フォルダまたはパターン | AI の運用に関するデータ | GitHub リポジトリ | パスの対応 |
|---|---|---|---|
| `Dropbox\ai` | `satsuki-thyme/ai` | `Dropbox\ai\` より後の相対パスを、区切りを `/` にしてリポジトリ内パスにする。 |

### その他

| Dropbox フォルダまたはパターン | 内容 | GitHub リポジトリ |
|---|---|---|
| `Dropbox\external-relations\等身大の点と点委員会` | 等身大の点と点委員会に関するデータ | `satsuki-thyme/life-sized-dot-to-dot-committee` |
| `Dropbox\www\satsuki` | 公式ホームページのデータ | `satsuki-thyme/satsuki` |
| `Dropbox` | 日常生活の管理 | なし |

### 趣味のプログラミング関連

| Dropbox フォルダまたはパターン | 内容 | GitHub リポジトリ |
|---|---|---|
| `Dropbox\www\studio\etc` | JavaScript などの小品 | `satsuki-thyme/etc` |
| `Dropbox\www\studio\common` | 複数の用途で共有するデータ | `satsuki-thyme/common` |
| `Dropbox\www\studio\brackettool.js` | 文書内の括弧を処理する JavaScript ライブラリ | `satsuki-thyme/brackettool.js` |
| `Dropbox\www\studio\comparearray.js` | 配列を比較する JavaScript ライブラリ | `satsuki-thyme/comparearray.js` |
| `Dropbox\www\studio\htmlshape.js` | HTML を整形する JavaScript ライブラリ | `satsuki-thyme/htmlshape.js` |
| `Dropbox\www\studio\maketable.js` | 配列からテーブルを生成する JavaScript ライブラリ | `satsuki-thyme/maketable.js` |
| `Dropbox\www\studio\mdparse.js` | Markdown を HTML に変換する JavaScript ライブラリ | `satsuki-thyme/mdparse.js` |
| `Dropbox\www\studio\notion-customization` | ユーザー CSS によって Notion の Web サイトをカスタマイズするためのデータ | `satsuki-thyme/notion-customization` |
| `Dropbox\www\studio\novelparse.js` | Web 小説の文書を HTML に変換する JavaScript ライブラリ | `satsuki-thyme/novelparse.js` |
| `Dropbox\www\studio\replacetool.js` | 文字列の置換処理を行う JavaScript ライブラリ | `satsuki-thyme/replacetool.js` |
| `Dropbox\www\studio\textodt.js` | テキストファイルを ODT 形式に変換する JavaScript ライブラリ | `satsuki-thyme/textodt.js` |
| `Dropbox\www\studio\wordcount.js` | 文字数を数える JavaScript ライブラリ | `satsuki-thyme/wordcount.js` |
| `Dropbox\www\studio\yamlparse.js` | YAML を Web 上で読みやすく表示する JavaScript ライブラリ | `satsuki-thyme/yamlparse.js` |

## GitHub リポジトリの対応

- この節のリポジトリはすべて GitHub アカウント `satsuki-thyme` のものとする。
- この対応は GitHub API で反映先候補を特定するために使う。更新前には、リポジトリの存在、書き込み権限、対象ブランチ、更新対象ファイルの対応を確認する。
- 表にない Dropbox フォルダ、または表の規則だけでリポジトリ内のファイルパスを確認できない場合は、推測で GitHub に変更を加えない。

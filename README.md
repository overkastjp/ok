# OVERKAST Brand

OVERKASTが公開するブランドテキストの置き場所です。Claude Codeで編集・更新することを前提に構成しています。

## 構成

```
ok/
├── README.md                    このファイル。目的と更新のしかた。
├── AGENTS.md                    AIの入口。ファイルの所在と、編集の原則。
├── CLAUDE.md                    互換ファイル。AGENTS.mdを読み込むだけ。
├── OVERKAST.md                  会社の一次情報。GitHub Rawで配信する公開ファイルなので直下に置く。
└── voice/
    ├── design-philosophy.md     デザイン思想の指示ファイル（旧版）。
    └── branding-diagnosis.md    ブランディング診断の指示ファイル（旧版）。
```

## Claude Codeでの使い方

このフォルダをルートとして開くと、Claude Codeは起動時に`CLAUDE.md`（を経由して`AGENTS.md`）を読み込みます。以降、ファイルを編集するときは、そこに書かれた編集と校正の原則にしたがいます。

編集を頼むときは、対象のファイルと、変えたいことを具体的に渡してください。たとえば「ok-brandの下書き（`thinking/obayashi/overkast-md-draft-2026-10.md`）の本文で、`OVERKAST.md`を置き換えて」。ここにない事実や数字は、ok-brandで決めてから渡してください。

## 更新のしかた

内容はok-brandで決め、ここへ反映します。ここで直接書き換えません。公開の手順は、`AGENTS.md`の「公開するとき」にまとめています。

- 内容を変えたら、frontmatterの`updated`を当日の日付にし、`version`を必要に応じて上げる。
- 公開ファイルは、frontmatterの`canonical_url`が指す場所に反映する。`main`に押すと、そのまま公開版になる。
- 押す前に`rule-check`を通し、大林が確認する。
- 何を変えたかは、コミットメッセージに一行で残す。過去の版は履歴でたどれる。

## 置くもの

ここには、公開するテキストだけを置きます。判断の決まり、作業の手順、決めたことの記録など、公開しないものはok-brandに置きます。

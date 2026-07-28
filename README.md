# OVERKAST Brand

OVERKASTが公開するブランドテキストの置き場所です。Claude Code で編集・更新することを前提に構成しています。

## 構成

```
overkast-brand/
├── README.md                    このファイル。目的と更新のしかた。
├── AGENTS.md                    AIの入口。ファイルの所在と、編集の原則。
├── CLAUDE.md                    互換ファイル。AGENTS.md を読み込むだけ。
├── context/
│   └── OVERKAST.md              会社の一次情報。判断の前提。
└── voice/
    ├── design-philosophy.md     デザイン思想の定義ファイル。
    └── branding-diagnosis.md    ブランディング診断ファイル。
```

## Claude Code での使い方

このフォルダをルートとして開くと、Claude Code は起動時に `CLAUDE.md`（を経由して `AGENTS.md`）を読み込みます。以降、ファイルを編集するときは、そこに書かれた〈文体〉と校正の原則にしたがいます。

編集を頼むときは、対象のファイルと、変えたいことを具体的に渡してください。たとえば「`context/OVERKAST.md` の ÉKRITS の節に、最新の書籍点数を反映して」。

## 更新のしかた

- 内容を変えたら、frontmatter の `updated` を当日の日付にし、`version` を必要に応じて上げる。
- 公開ファイルは、frontmatter の `canonical_url` が指す場所に反映する。
- 何を変えたかは、コミットメッセージに一行で残す。過去の版は履歴でたどれる。

## この先の拡張

いまは公開テキストだけを置いています。運用が進んだら、次を足せます。

- `rules/` — 場面ごとの判断ルール（営業、問い合わせ対応など）。
- `skills/` — 定型作業の手順（提案書の書き方など）。
- `examples/` — よい出力と、そうでない出力の例。
- `memory/` — 運用のなかで蓄積される文脈。

これは、OVERKAST がクライアントに渡す構成と同じ考え方です。仕組みだけ先に用意し、中身は使いながら育てます。

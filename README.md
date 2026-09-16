# tebanare.jp 転送ページ

`tebanare.jp` を `https://tebanare.rstreet.co.jp/`（テバナレ｜経理AIエージェント のLP）へ転送するだけのリポジトリ。

- ドメインは 2026-09-16 に株式会社アールストリート名義で取得（お名前.com、保険目的）。LP 本体はコーポレートの権威性を引き継ぐサブドメインに置く方針のため、ここには中身を置かない
- 転送は `index.html` の `meta refresh` + `location.replace`（パスに関係なく LP のトップへ）。`noindex` と `canonical` で索引には入れない
- 配信は GitHub Pages（main ブランチ直下）。カスタムドメインは `CNAME`
- DNS（お名前.com の DNS レコード設定）: `@` の A レコード 4 本 → 185.199.108.153 / 185.199.109.153 / 185.199.110.153 / 185.199.111.153、`www` の CNAME → r-street-jp.github.io
- 記録: corporate-site-ops `tebanare/playbook/2026-09_lp_seo_foundation.md`

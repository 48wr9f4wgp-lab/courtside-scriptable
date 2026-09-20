# COURTSIDE / Scriptable

推しNBAチーム専用ウィジェット。

## 運用

Scriptable側には `LOADER.js` だけを置く。

- Loader: `LOADER.js`
- Remote app: `COURTSIDE.js`
- Default branch: `main`

Loaderは毎回GitHub上の `COURTSIDE.js` を取得して実行する。
取得成功時は端末へキャッシュし、GitHub取得に失敗した場合は最後に取得できたコードへフォールバックする。

これ以降の通常更新は `COURTSIDE.js` のみ変更する。
Loader自体の再貼り付けは、Loader方式そのものを変更する場合だけ必要。

## Team

Scriptable Widget ParameterへNBA略称を設定する。

例:

- LAL
- GSW
- BOS
- NYK
- MIA

未指定時は `LAL`。

## Current

- Remote app: COURTSIDE v0.4.1
- Loader: v1.1
- Repository: `48wr9f4wgp-lab/courtside-scriptable`
- Status: 専用Repositoryへ移設済み / Scriptable loader経由の実機検証待ち

## Data

現行prototypeはESPNのpublic-facing JSON endpointを利用。
公式developer APIとして保証されたendpointではないため、仕様変更時は取得層を差し替える。


## Verification

- Medium preview: VERIFIED on iPhone
- Small preview: VERIFIED on iPhone
- Large preview: VERIFIED on iPhone
- Lock Screen previews: PENDING

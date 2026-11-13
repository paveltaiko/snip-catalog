# Snip – katalog služeb

Podepsaný katalog předplatných pro aplikaci [Snip](https://github.com/paveltaiko/Snip).

- `v1/catalog.json` – seznam služeb, kategorií, odkazů na zrušení a ověřených tarifů
- `v1/catalog.json.sig` – podpis Ed25519 (base64)

Aplikace si katalog jednou denně stáhne a přijme ho jen tehdy, když podpis sedí
na veřejný klíč zabudovaný v aplikaci a verze je novější než ta, kterou už má.

Obsahuje jen veřejné informace o službách – žádná uživatelská data.

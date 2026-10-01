---
'incur': patch
---

Surface `error.code` and `error.message` from nested `{ error: { code, message } }` response bodies in OpenAPI-generated commands and the fetch gateway, instead of falling back to `HTTP <status>`.

---
'incur': minor
---

Added `openapiConfig.groupsFromTags` to describe namespace-mode command groups from the OpenAPI document's tag descriptions.

```ts
Cli.create('my-cli').command('api', {
  fetch: app.fetch,
  openapi: spec,
  openapiConfig: { groupsFromTags: true, mode: 'namespace' },
})
```

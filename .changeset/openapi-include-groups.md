---
'incur': minor
---

Added `openapiConfig.include` to generate commands for only the operations it matches, and `openapiConfig.groups` to describe generated command groups.

```ts
Cli.create('my-cli').command('api', {
  fetch: app.fetch,
  openapi: spec,
  openapiConfig: {
    groups: { users: 'Manage users' },
    include: (o) => o.path.startsWith('/users'),
    mode: 'namespace',
  },
})
```

# Pocketenv Docs

Official documentation for [Pocketenv](https://pocketenv.io) — open-source, multi-provider sandbox platform.

Built with [Mintlify](https://mintlify.com) and published at **[docs.pocketenv.io](https://docs.pocketenv.io)**.

## What's inside

```
.
├── index.mdx                  # Landing page
├── quickstart.mdx             # Install CLI & create first sandbox
├── development.mdx            # SDK overview
├── guides/
│   ├── providers.mdx          # Supported backend providers
│   ├── exec-and-console.mdx   # Running commands & interactive shell
│   ├── secrets-and-env.mdx    # Secrets & environment variables
│   ├── ports-and-networking.mdx
│   ├── services.mdx
│   └── backups.mdx
├── sdks/
│   ├── javascript.mdx         # @pocketenv/sdk (JS/TS)
│   ├── gleam.mdx
│   ├── clojure.mdx
│   └── elixir.mdx
└── api-reference/
    ├── introduction.mdx
    ├── openapi.json            # XRPC OpenAPI spec
    ├── actor/
    ├── sandbox/
    ├── file/
    ├── secret/
    ├── variable/
    ├── service/
    └── volume/
```

## Local development

Install the Mintlify CLI:

```sh
npm i -g mint
```

Run the local preview server from the root of this repo (where `docs.json` is):

```sh
mint dev
```

Open [http://localhost:3000](http://localhost:3000).

## Contributing

1. Fork & clone the repo
2. Run `mint dev` to preview changes locally
3. Edit or add `.mdx` files — pages map 1:1 to files
4. Update `docs.json` if you add or move pages
5. Open a pull request

### Adding a page

Create an `.mdx` file and add its path to the relevant `group` in `docs.json`:

```json
{
  "group": "Guides",
  "pages": ["guides/your-new-page"]
}
```

### API reference pages

API pages are generated from `api-reference/openapi.json`. Each page is a single MDX file with an `openapi` frontmatter field:

```mdx
---
title: 'Create Sandbox'
openapi: 'POST /io.pocketenv.sandbox.createSandbox'
---
```

## Related repos

| Repo | Description |
|---|---|
| [pocketenv-io/pocketenv](https://github.com/pocketenv-io/pocketenv) | Core platform & CLI |
| [pocketenv-io/pocketenv-js](https://github.com/pocketenv-io/pocketenv-js) | JavaScript / TypeScript SDK |
| [pocketenv-io/pocketenv-gleam](https://github.com/pocketenv-io/pocketenv-gleam) | Gleam SDK |
| [pocketenv-io/pocketenv-clojure](https://github.com/pocketenv-io/pocketenv-clojure) | Clojure SDK |
| [pocketenv-io/pocketenv-elixir](https://github.com/pocketenv-io/pocketenv-elixir) | Elixir SDK |

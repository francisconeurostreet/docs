# Ignite API docs

This repository contains the public Mintlify documentation for Ignite API.

The site includes:

- Overview and quickstart pages in MDX
- A public changelog
- An OpenAPI-powered API reference from `openapi.json`
- Mintlify site configuration in `docs.json`

## Editing

Pages are MDX files. Keep docs concise, use active voice, and format file names, commands, paths, and API fields with code formatting.

Do not change endpoint contracts in `openapi.json` from this repo unless the API source of truth has already changed. Metadata-only cleanup is fine.

## Local preview

Install the Mintlify CLI if needed:

```
npm i -g mint
```

Run the preview from the repository root:

```
mint dev
```

View your local preview at `http://localhost:3000`.

## Checks

Before publishing, validate the JSON files:

```
python3 -m json.tool docs.json
python3 -m json.tool openapi.json
```

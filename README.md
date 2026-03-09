# crawler

Monorepo for social/video crawling tools and MCP integrations.

## Packages

- `packages/video-download-mcp`: MCP server for resolving and downloading videos from share links.

## Quick Start

```bash
cd packages/video-download-mcp
npm install
npm run build
npm run serve
```

## Claude Code Integration

After publishing `@cory-ronghua/video-fetch-mcp` to npm:

```bash
claude mcp add video-fetch-mcp -- npx -y @cory-ronghua/video-fetch-mcp
```

## Publishing

This repository uses npm Trusted Publishing via GitHub Actions:

- Workflow: `.github/workflows/publish-video-download-mcp.yml`
- Trigger: GitHub Release `published`
- Publish command: `npm publish --provenance --access public`

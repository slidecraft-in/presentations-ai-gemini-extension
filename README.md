# Presentations.AI — Gemini CLI Extension

Create designed presentations, slide decks, and single slides from a topic,
raw text, or a source document — directly from the Gemini CLI.

Backed by the [Presentations.AI MCP server](https://api.presentations.ai/mcp)
with OAuth 2.0 authentication (PKCE + Dynamic Client Registration).

## What you get

5 MCP tools available inside Gemini CLI:

- `create_presentation_from_topic` — full deck from a brief
- `create_single_slide` — single image slide from a topic
- `create_presentation_from_content` — deck from raw text (article, notes, transcript)
- `create_presentation_from_file` — deck from PDF, DOCX, PPTX, TXT, or MD (≤ 5 MB)
- `check_job_status` — poll long-running async jobs

## Install

```bash
gemini extensions install https://github.com/slidecraft-in/presentations-ai-gemini-extension
```

On first use, Gemini CLI opens a browser for OAuth sign-in to your
Presentations.AI account. A Presentations.AI account is required.

## Usage

```
> create a 10-slide pitch deck on quantum computing for executives
> turn this article into a 12-slide deck: <paste text>
> make a single slide explaining transformers
```

## Account

Sign up at [presentations.ai](https://presentations.ai). API access requires a
plan that includes it — see [console.presentations.ai/apiref/docs](https://console.presentations.ai/apiref/docs/).

## Support

Email: `support@presentations.ai`

## License

MIT — see [LICENSE](LICENSE).

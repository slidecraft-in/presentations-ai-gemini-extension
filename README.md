# Presentations.AI for Gemini CLI

Create designed slide decks with [Presentations.AI](https://www.presentations.ai) from Gemini
CLI, then download, share, or manage them.

The extension adds:

- the Presentations.AI MCP server, `https://api.presentations.ai/mcp`;
- two [agent skills](https://geminicli.com/docs/cli/skills/), `create-presentation` and
  `manage-presentations`, that guide Gemini through making a deck and managing existing ones;
- `GEMINI.md`, a short context file that points Gemini to those skills.

## Install

```bash
gemini extensions install https://github.com/slidecraft-in/presentations-ai-gemini-extension
```

A Presentations.AI account is required. The first time Gemini CLI connects, it registers
itself with the server and opens a browser for you to sign in. If you need to sign in again,
run `/mcp auth presentations-ai`.

## Tools

| Tool | Use it to |
|---|---|
| `create_presentation` | Generate a deck from a prompt, pasted text, or an edited outline, with optional audience, slide count, and brand kit. |
| `create_outline` | Draft an outline to review and edit before generating. Spends credits: 10 per slide. |
| `get_task` | Wait up to 60 s per call for generation to finish. |
| `get_export` | A download link for the finished file, valid for 15 minutes. |
| `share_deck` | A public link anyone can open, created when the user asks to share. |
| `search_brand_kits` | Find a brand to apply via `brand_kit_id`. |
| `whoami` | Identity, workspace, plan, and credit balance. |
| `list_decks` / `get_deck` / `list_projects` | Find and inspect existing work. |
| `patch_deck` / `delete_deck` | Rename, move, change visibility or content version, or delete a deck. |
| `create_grant` | Share a deck with a person by email. |

## Examples

```
> make a 10-slide pitch deck on our Q3 results for the leadership team
> turn these meeting notes into a short deck: <paste text>
> show me an outline first, then build the deck with the Presentations.AI brand kit
> share my "Q3 results" deck with teammate@example.com as a viewer
```

## Support

- Docs: [docs.presentations.ai/docs/agents](https://docs.presentations.ai/docs/agents)
- Email: `support@presentations.ai`

## License

MIT, see [LICENSE](LICENSE).

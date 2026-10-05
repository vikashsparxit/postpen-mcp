<p align="center"><img src="logo.png" width="96" alt="PostPen logo"></p>

# PostPen MCP Server

Schedule and publish LinkedIn posts from your AI agent through [PostPen](https://postpen.ai).

PostPen lets your AI agent publish to LinkedIn for you. The agent writes the post. PostPen holds your LinkedIn connection, saves drafts, attaches images, videos, or PDF carousels, schedules posts for the time you choose, and publishes them to your personal profile or to company pages your plan includes.

You connect LinkedIn once inside PostPen. Your agent signs in to PostPen through your browser (OAuth) and never sees your LinkedIn token. Every post lands on your PostPen calendar, where you can review, edit, or move it before it goes out. Publishing immediately and deleting drafts require an explicit confirmation from the agent.

This is a hosted remote server. There is nothing to install or run locally.

## Connect

- **Server URL:** `https://mcp.postpen.ai`
- **Transport:** Streamable HTTP
- **Auth:** OAuth 2.0 (sign in to PostPen in your browser; dynamic client registration supported)
- **Official MCP Registry:** `ai.postpen/postpen`

### Cursor / VS Code / Windsurf / other JSON-config clients

```json
{
  "mcpServers": {
    "postpen": {
      "url": "https://mcp.postpen.ai"
    }
  }
}
```

### Claude, ChatGPT, Grok and other apps with custom connectors

Add a custom connector and paste `https://mcp.postpen.ai`, then sign in to PostPen when prompted.

## Tools

| Tool | What it does |
|---|---|
| `list_destinations` | List your LinkedIn profile and company pages |
| `list_posts` | List drafts, scheduled and sent posts |
| `save_draft` | Create or update a draft |
| `create_upload` | Upload an image, video or PDF carousel |
| `schedule_post` | Schedule a post for a specific time |
| `unschedule_post` | Move a scheduled post back to drafts |
| `delete_draft` | Delete an unpublished draft (requires confirmation) |
| `publish_now` | Publish to LinkedIn immediately (requires confirmation) |

## Requirements

A PostPen account with LinkedIn connected. Company pages need the Organization or Enterprise plan. This server posts only to LinkedIn.

## Links

- Website: https://postpen.ai
- Connect an agent: https://app.postpen.ai/agents
- Support: https://postpen.ai/support
- Privacy: https://postpen.ai/privacy-policy
- Terms: https://postpen.ai/terms-of-service
- Contact: hello@postpen.ai

PostPen is built by SparxIT (Sparx IT Solutions Private Limited). LinkedIn is a trademark of LinkedIn Corporation; PostPen is not affiliated with LinkedIn.

This repository is the PostPen Cursor plugin package and install documentation (manifest, MCP config, docs and logos), released under the MIT License. The hosted PostPen server and app at mcp.postpen.ai are proprietary and not covered by this license.

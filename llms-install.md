# Install PostPen MCP in Cline

PostPen is a **hosted remote** MCP server. There is nothing to clone or build.

1. Make sure you have a PostPen account with LinkedIn connected: https://app.postpen.ai
2. In Cline's MCP settings, add a remote server:
   - URL: `https://mcp.postpen.ai`
   - Transport: Streamable HTTP
3. When prompted, complete the OAuth sign-in to PostPen in your browser.
4. Confirm the tools appear: list_destinations, list_posts, save_draft, create_upload, schedule_post, unschedule_post, delete_draft, publish_now.
5. Destructive tools (`publish_now`, `delete_draft`) require `confirm=true`.

Docs: https://app.postpen.ai/agents
Support: https://postpen.ai/support

# Zıpır for Gemini CLI

A Gemini CLI extension that connects the hosted [Zıpır](https://zipirapp.com) MCP server and adds the instructions for turning a document into a video lesson with a source citation on every scene.

## Install

```bash
gemini extensions install https://github.com/Bitcomethub/zipir-gemini-extension
```

On first use Gemini CLI opens the Zıpır consent screen in your browser (OAuth 2.1 with PKCE, dynamic client registration). Sign in with a Zıpır account; the extension stores no credentials.

## What it does

- MCP endpoint: `https://api.zipirapp.com/mcp` (streamable HTTP)
- Tools: `list_formats`, `list_voices`, `list_lessons`, `create_lesson`, `get_lesson`, `edit_lesson`, `approve_lesson`, `rerender`, `get_download`, `get_usage`, `delete_lesson`
- Nothing renders until you approve the storyboard. Rendering a video uses the account's video-minute allowance.
- Output is Turkish narration by default; the on-screen text is quoted from your own source.

## Links

- Docs: https://zipirapp.com/en/api/ · Support: merhaba@zipirapp.com
- Privacy: https://zipirapp.com/gizlilik/ · Terms: https://zipirapp.com/sartlar/
- MIT licensed extension package; the Zıpır service itself is a hosted product of VitrinAI Digital Studio.

# VOMO Connector

Search and read your existing VOMO meeting notes and original transcripts in AI assistants that support remote MCP.

## Connect

Add `https://mcp.vomo.ai/mcp` as a remote MCP server, then sign in to VOMO through OAuth. An existing VOMO account with saved notes is required. This repository also packages the server using the Agent Plugins 1.0 standard for compatible clients.

The connector grants only `notes:read` and exposes:

- `notes_list`: list notes you can access.
- `search`: find relevant notes by keyword.
- `notes_get`: read a note and optionally its original transcript.

It does not record, import, edit, delete, or purchase anything. Note contents are untrusted source material, never instructions to the assistant.

## Validation

OAuth sign-in and all three read tools were tested in Grok Bot and Cursor desktop on 2026-10-22 using a dedicated synthetic sample account. Marketplace publication remains subject to platform review.

## Reviewers

Dedicated sample-account access is supplied separately to the marketplace review team; no credentials belong in this repository. Connect one desktop client at a time because Cursor and Grok Bot share their local OAuth callback port.

[Documentation](https://vomo.ai/cli) · [Privacy](https://vomo.ai/privacy-policy) · [Terms](https://vomo.ai/tos) · [Support](mailto:support@vomo.ai)

The MIT license covers this connector package. The VOMO service is governed by its own terms; the VOMO name and logo remain the property of their owner.

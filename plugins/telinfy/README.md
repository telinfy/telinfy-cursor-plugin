# Telinfy for Cursor

Connect Cursor to [Telinfy](https://telinfy.com), the messaging platform by GreenAds Global. Ask Cursor's agent to send and schedule SMS and WhatsApp campaigns, manage phonebooks, and pull delivery reports from your Telinfy account.

## What's included

| Component | What it does |
|---|---|
| MCP server `telinfy` | Remote server at `https://mcp.telinfy.com` with 15 tools for SMS, WhatsApp, RCS reports and phonebooks |
| Rule `telinfy-messaging` | Guides the agent to confirm before sending, respect opt-outs, and verify delivery |

## Setup

1. Install the plugin.
2. Cursor shows **Needs authentication** next to the Telinfy server. Click **Authenticate**.
3. Sign in with your Telinfy username and password in the browser window that opens.
4. Try: *"Show my Telinfy phonebook groups."*

You need a Telinfy account. Sign up at [telinfy.com](https://telinfy.com).

## Tools

- **SMS:** `send_sms`, `schedule_sms`, `fetch_sms_campaign_report`, `get_sms_schedule`, `getMessageReport`
- **WhatsApp:** `send_whatsapp_campaign`, `whatsapp_campaign`, `fetch_whatsapp_smart_report`
- **RCS:** `fetch_rcs_report`
- **Phonebook:** `create_phonebook`, `get_phonebook_groups`, `get_group_contacts`, `edit_contact`, `toggle_contact_status`, `delete_contact_group`

## Consent

Sends only reach contacts saved and active in your Telinfy phonebook. The server checks every recipient and refuses any number that isn't an opted-in contact. Deactivating a contact in any group records an opt-out.

## Prerequisites for sending

- **SMS to India:** a DLT-registered sender ID and approved DLT template IDs. Message text must match the registered template.
- **WhatsApp:** an approved WhatsApp Business template on your Telinfy account.

## Privacy and security

Sign-in uses OAuth 2.0 with PKCE. Your password goes only to Telinfy's login service; it is never stored by the server or shared with Cursor. Access tokens last up to 8 hours.

- Documentation and troubleshooting: https://mcp.telinfy.com/docs
- Privacy policy: https://www.greenadsglobal.com/privacy-policy
- Support: support@telinfy.com

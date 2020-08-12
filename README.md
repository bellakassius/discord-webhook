# Discord Webhook Action

This will send a message to a discord webhook.

## Inputs

| Name | Required | Description |
|------|----------|-------------|
| webhook-url | `true`        |  Webhook URL from discord. See: https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks for details           |
| content    | `true`       | Message that is send via the webhook.            |
| username    | `true`       |  The username that should appear to send the message. Note: username will have the "bot" badge next to their name.           |
| avatar-url | `true` | URL for the avatar that should appear with the message. |

## Example Usage

```yaml
uses: actions/discord-webhook@v1
with:
    webhook-url: https://discordapp.com/api/webhooks/<webhook_id>/<webhook_token>
    content: Hello, world!
    username: Botty McBotface
    avatar-url: <some_image_url>
```

## Todo

- Make `username` and `avatar-url` optional

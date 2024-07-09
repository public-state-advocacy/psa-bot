# psa-tg-bot

## High Level Functionality

The bot has 2 primary functions:
- Allow users to submit an application to join PSA
- Allow a PSA admin to approve an application and auto add a user to PSA TG channel

## Local Development

Install deps

```bash
npm i
```

Generate your [telegram bot](https://core.telegram.org/bots/tutorial) for local dev.

Create a [smee channel](https://smee.io/new) to proxy webhook requests to your local server. Copy the generated smee channel url as you'll need to save it as `DELPHI_READS_WEBHOOK_URL` in your `.env` file.

Copy `.env.template` to `.env` file:

```bash
cp .env.template .env
```

Open `.env` and populate values.

Start the server in dev mode:

```bash
npm run start:dev
```

Dev mode will automatically configure smee to proxy requests to your local server.

## Bot Commands

Use BotFather to set commands for your bot.

1. In conversation with BotFather:

```
/setcommands
```

2. Then, select the bot to set commands for

3. Finally, add all your commands. Below could be used for the Delphi Reads bot:

```
...tbd
```

## Deployment


```
# deploy to beta/staging environment
npm run deploy

# deploy to prod
npm run deploy:prod
```

## Resources

[Telegraf Docs](https://github.com/feathers-studio/telegraf-docs)

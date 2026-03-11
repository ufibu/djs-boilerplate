# djs-boilerplate

CLI tool to scaffold Discord.js bot projects. Born out of my own need — I build a lot of Discord bots and got tired of setting up the same boilerplate every time.

## Usage

```bash
npx djs-boilerplate my-bot
```

## Features

- TypeScript or JavaScript
- Slash commands, prefix commands, or both
- Optional `src/` folder structure
- MongoDB integration (optional)
- Dynamic event and command handler
- Example helper system (e.g. ticket system)

## What you get

```
my-bot/
├── commands/
│   ├── slash/
│   └── prefix/
├── events/
│   └── discord/
├── handlers/
│   ├── events.ts
│   ├── commands.ts
│   ├── helpers.ts
│   └── manager/
├── helpers/
├── models/
├── types/
├── utils/
└── index.ts
```

## Options

| Prompt | Choices |
|---|---|
| Package manager | npm, pnpm, bun |
| Language | TypeScript, JavaScript |
| Command style | Slash, Prefix, Both |
| src/ folder | Yes, No |
| Database | None, MongoDB |

## After scaffolding

```bash
cd my-bot
cp .env.example .env
# Add your bot token to .env
pnpm dev
```

To register slash commands:

```bash
pnpm deploy
```

## License

MIT

# chatHSKN
# Discord ChatGPT Bot

A Discord bot that integrates with ChatGPT for conversational AI interactions.

## Prerequisites

- Node.js (v16 or higher)
- A Discord Bot Token (from [Discord Developer Portal](https://discord.com/developers/applications))
- An OpenAI API Key (from [OpenAI Platform](https://platform.openai.com/api-keys))

## Installation

1. Clone or download this repository
2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with your tokens:
```
DISCORD_TOKEN=your_discord_bot_token_here
OPENAI_API_KEY=your_openai_api_key_here
```

4. Start the bot:
```bash
node src/index.js
```

## Usage

The bot responds to the following commands:
- `!chat <message>` - Chat with the AI
- `!help` - Show available commands

## Important Notes

- Enable these privileged intents in the Discord Developer Portal:
  - MESSAGE CONTENT INTENT
  - SERVER MEMBERS INTENT
  - PRESENCE INTENT

- The bot includes rate limiting (5 requests per minute per user)
- Responses are automatically split if they exceed Discord's message length limit

## Dependencies

- discord.js
- openai
- dotenv

## Support

For issues with:
- Discord Bot Token: Visit the [Discord Developer Portal](https://discord.com/developers/applications)
- OpenAI API: Check [OpenAI's Documentation](https://platform.openai.com/docs)

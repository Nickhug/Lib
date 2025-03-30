# LobeChat Custom Marketplace

This repository contains custom marketplace files for LobeChat, featuring real estate focused assistants and plugins.

## Repository Structure

```
Lib/
├── agents/
│   ├── index.en-US.json              # List of all assistants
│   ├── discover-home.en-US.json      # Home page featured assistants
│   ├── realtor-assistant.en-US.json  # Realtor Assistant definition
│   └── finance-expert.en-US.json     # Finance Expert definition
├── plugins/
│   └── index.en-US.json              # List of all plugins
├── models/
│   └── index.en-US.json              # List of all models
└── providers/
    └── index.en-US.json              # List of all providers
```

## Setup Instructions

1. Clone this repository
2. Add your custom assistants and plugins by editing the JSON files
3. Push changes to GitHub
4. Set these environment variables in your LobeChat deployment:

```
AGENTS_INDEX_URL=https://raw.githubusercontent.com/Nickhug/Lib/main/agents
PLUGINS_INDEX_URL=https://raw.githubusercontent.com/Nickhug/Lib/main/plugins
MODELS_INDEX_URL=https://raw.githubusercontent.com/Nickhug/Lib/main/models
PROVIDER_INDEX_URL=https://raw.githubusercontent.com/Nickhug/Lib/main/providers
```

## Available Assistants

- **Realtor Assistant**: AI-powered real estate assistant for property analysis
- **Finance Expert**: Financial analyst providing investment advice

## Available Plugins

- **Real Estate Lookup**: Search for real estate properties and market data
- **Web Crawler**: Access web content with URL support

## Adding More Assistants

To add a new assistant:

1. Add it to `agents/index.en-US.json`
2. Create a new file `agents/your-assistant-name.en-US.json`

## Adding More Plugins

To add a new plugin, edit the `plugins/index.en-US.json` file.

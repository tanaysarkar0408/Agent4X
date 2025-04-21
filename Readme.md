# AI Agent for X (formerly Twitter) with MCP Server

This project is an AI-powered agent that integrates with the Model Context Protocol (MCP) server to perform various tasks, including posting updates to X (formerly Twitter). The agent uses tools defined on the MCP server and communicates with the server via SSE (Server-Sent Events).

## Features

- Post updates to X (formerly Twitter) using the `createPost` tool.
- AI-driven chat interface powered by Google GenAI.
- Dynamic tool discovery and execution via the MCP protocol.

## Prerequisites

- Node.js (v16 or later)
- Twitter Developer Account
- Google GenAI API Key
- `.env` file with the required API keys and secrets.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd MCP
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add the following environment variables:
   ```
   TWITTER_API_KEY=<your-twitter-api-key>
   TWITTER_API_SECRET=<your-twitter-api-secret>
   TWITTER_ACCESS_TOKEN=<your-twitter-access-token>
   TWITTER_ACCESS_TOKEN_SECRET=<your-twitter-access-token-secret>
   GEMINI_API_KEY=<your-google-genai-api-key>
   ```

4. Start the MCP server:
   ```bash
   node Server/Index.js
   ```

5. Start the client:
   ```bash
   node Client/Index.js
   ```

## Generating Twitter API Tokens and Secret Keys

To use the `createPost` tool, you need to generate Twitter API tokens and secret keys. Follow these steps:

1. Go to the [Twitter Developer Portal](https://developer.twitter.com/).
2. Log in with your Twitter account and create a new project.
3. Under your project, create a new app.
4. Navigate to the "Keys and Tokens" section of your app.
5. Generate the following keys and tokens:
   - API Key
   - API Key Secret
   - Access Token
   - Access Token Secret
6. Copy these values and add them to your `.env` file as shown above.

## Usage

- The server exposes tools like `createPost` for posting updates to X.
- The client connects to the server, discovers available tools, and uses AI to interact with the user.
- Use the chat interface to ask questions or trigger tool executions.

## License

This project is licensed under ME(HAHAHA😂).

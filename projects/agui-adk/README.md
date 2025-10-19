# CopilotKit <> ADK Starter 🤖

Build AI agents using Google's ADK and CopilotKit - create intelligent investment analyst agents that research stocks, analyze market data, and provide investment insights.

## Why This Matters

- 🏠 **Local Development**: Complete AI agent development environment with Next.js and Python
- 🧠 **Google ADK**: Leverage Google's Agent Development Kit for powerful AI capabilities
- 🚀 **CopilotKit Integration**: Modern React components for seamless AI agent interactions
- 📊 **Investment Focus**: Pre-built investment analyst agent for financial data analysis
- 💰 **Production Ready**: Scalable architecture for real-world AI applications

## Key Features

- **Investment Analyst Agent**: Research stocks and analyze market data
- **Modern UI**: Next.js application with CopilotKit sidebar integration
- **Dual Server Architecture**: Separate UI and agent servers for optimal performance
- **Multiple Package Managers**: Support for pnpm, npm, yarn, and bun
- **Debug Mode**: Enhanced logging for development and troubleshooting

## Installation and Setup

### Prerequisites
- Node.js 18+
- Python 3.12+
- Google Makersuite API Key ([Get yours here](https://makersuite.google.com/app/apikey))
- Package manager: pnpm (recommended), npm, yarn, or bun

### 1. Install Dependencies

**Frontend dependencies:**
```bash
# Using pnpm (recommended)
pnpm install

# Using npm
npm install

# Using yarn
yarn install

# Using bun
bun install
```

**Python agent dependencies:**
```bash
# Using pnpm
pnpm install:agent

# Using npm
npm run install:agent

# Using yarn
yarn install:agent

# Using bun
bun run install:agent
```

### 2. Set Up Google API Key

```bash
export GOOGLE_API_KEY="your-google-api-key-here"
```

### 3. Run the Application

```bash
# Using pnpm
pnpm dev

# Using npm
npm run dev

# Using yarn
yarn dev

# Using bun
bun run dev
```

The application will be available at `http://localhost:3000` with the agent server running on port 8000.

## Project Structure

```
agui-adk/
├── src/
│   └── app/
│       └── page.tsx         # Main UI component
├── agent/
│   ├── .venv/              # Python virtual environment
│   └── requirements.txt    # Python dependencies
├── package.json            # Node.js dependencies and scripts
└── README.md
```

## Available Scripts

- `dev` - Starts both UI and agent servers in development mode
- `dev:debug` - Starts development servers with debug logging enabled
- `dev:ui` - Starts only the Next.js UI server
- `dev:agent` - Starts only the ADK agent server
- `build` - Builds the Next.js application for production
- `start` - Starts the production server
- `lint` - Runs ESLint for code linting
- `install:agent` - Installs Python dependencies for the agent

## Usage

1. Start the development servers using `pnpm dev`
2. Open your browser to `http://localhost:3000`
3. Interact with the investment analyst agent through the CopilotKit sidebar
4. Ask questions about stocks, market analysis, or investment strategies
5. Customize the agent behavior by modifying the ADK configuration

## Troubleshooting

### Agent Connection Issues
If you see "I'm having trouble connecting to my tools":
1. Ensure the ADK agent is running on port 8000
2. Verify your Google API key is set correctly
3. Check that both servers started successfully

### Python Dependencies
If you encounter Python import errors:
```bash
cd agent
pip install -r requirements.txt
```

---

## Contribution

Contributions are welcome! Please fork the repository and submit a pull request with your improvements.
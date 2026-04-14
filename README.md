# Forge

A modern Solana decentralized application (dApp) starter built with Next.js, Tailwind CSS, `@solana/kit`, and an Anchor vault program.

> **Note:** This project is currently under active development. More details will be added here soon.

## 🚀 Quick Start

### Prerequisites

- Node.js (v18+)
- [Rust](https://rustup.rs/)
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools)
- [Anchor Framework](https://www.anchor-lang.com/docs/installation)

### Setup & Run

```bash
# Install dependencies
npm install

# Build the Anchor program and generate the TypeScript client
npm run setup

# Start the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the application.

## 🏗️ Project Structure

- **`app/`**: Next.js frontend code (React components, hooks, styles, providers)
- **`anchor/`**: Solana smart contract workspace (Rust programs, tests)
- **`codama.json`**: Configuration for `codama` JS client generation

## 🛠️ Available Scripts

- `npm run dev`: Starts the Next.js development server
- `npm run build`: Builds the Next.js application for production
- `npm run setup`: Builds the Anchor program and regenerates the TypeScript client
- `npm run anchor-build`: Compiles the Anchor program
- `npm run anchor-test`: Runs smart contract tests against LiteSVM
- `npm run codama:js`: Regenerates the TypeScript client from the Anchor IDL

## 🔧 Local Development

1. Start a local Solana validator:
   ```bash
   solana-test-validator
   ```
2. Deploy the program locally:
   ```bash
   solana config set --url localhost
   anchor build
   anchor deploy
   npm run codama:js
   ```
3. Switch your app to use `localnet` in the connected wallet or Next.js UI container.

## 🔗 Learn More

- [Solana Docs](https://solana.com/docs)
- [Anchor Docs](https://www.anchor-lang.com/docs/introduction)
- [@solana/kit](https://github.com/anza-xyz/kit)

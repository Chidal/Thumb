# Thumb
**Built for**: Production-grade Farcaster Mini Apps on Celo  

## Overview

**Thumb** is a real-time, AI-powered onchain events dashboard designed as a high-performance Farcaster Mini App running natively on **Celo** — the fastest, cheapest, and most mobile-friendly EVM chain.

Thumb delivers instant, beautiful, and intelligent insights into Celo blockchain activity (transactions, blocks, wallets, and social signals) directly inside Warpcast and other Farcaster clients via **Frames v2** and **Mini Apps**. It combines live event streaming, AI-driven summarization, anomaly detection, and predictive analytics — all wrapped in a sleek, degen-style UI that feels native in Farcaster.

Built as a production-grade reference implementation, **Thumb** accelerates the creation of next-generation social-first dApps by showcasing best practices for Farcaster Frames, MiniKit, Celo’s 1-second finality, and ultra-low gas.

Live contract on Celo Mainnet:  
`0xd9aC52cCaD325f96398A06ADad409B30b3768d24`  
Explorer: https://celoscan.io/address/0xd9aC52cCaD325f96398A06ADad409B30b3768d24

Launch Thumb in Warpcast → **thumb.fcast.me**

---

## Features

- **Native Farcaster Mini App** – Full-screen, instant-launch experience inside Warpcast
- **Frames v2 Powered Entry** – Start from any cast with one tap
- **Real-Time Onchain Feed** – Live Celo transactions, mints, transfers, and social actions
- **AI-Powered Insights** – Natural language summaries (“12 cUSD tips in the last 10 mins”), anomaly alerts (“Whale just moved 50k cREAL”), and trend predictions
- **Social-First Interactions** – One-tap onchain reactions, tips, follows, and collects via MiniKit
- **Developer Dashboard (`/nerds`)** – Raw + decoded event logs for builders
- **Gamified UI** – Interactive charts, live leaderboards, and prediction games
- **Zero-Friction Wallet** – MiniKit + RainbowKit for seamless sign-in and transactions

---

## Tech Stack

- **Frontend**:
  - **Next.js (App Router)** – Optimized for Farcaster Mini Apps + edge deployment
  - **Tailwind CSS** – Fast, beautiful, mobile-perfect design
  - **TypeScript** – Full type safety across onchain + Farcaster data
  - **Chart.js + Recharts** – Smooth, interactive onchain visualizations
  - **Framer Motion** – Buttery animations that feel native
- **Farcaster Technologies**:
  - **Frames v2** – Entry point from any cast
  - **MiniKit** – Wallet, transactions, notifications, storage
  - **Farcaster Hubs** – Real-time cast and reaction streaming
- **Blockchain**:
  - **Celo Mainnet / Alfajores** – 1-second finality, sub-cent fees, phone-number addresses
  - **Viem + Wagmi** – Lightweight, modern blockchain primitives
  - **MiniKit SDK** – Native Farcaster wallet + tx handling
- **Real-Time**:
  - **Celo Indexers + Webhooks** – Sub-second event streaming
  - **Server-Sent Events (SSE)** – Live updates inside the Mini App
- **Deployment**:
  - **Vercel** – Edge-deployed, globally fast, Mini App-optimized

---

## Getting Started

### Run Locally

```bash
git clone https://github.com/Chidal/thumb.git
cd thumb
npm install
```

Create `.env.local`:

```env
NEXT_PUBLIC_CELO_RPC=https://forno.celo.org
NEXT_PUBLIC_ALFAJORES_RPC=https://alfajores-forno.celo-testnet.org
NEXT_PUBLIC_WALLETCONNECT_PROJECT_ID=your_id_here
```

```bash
npm run dev
```

Open in Warpcast using this Frame URL:
`https://thumb.fcast.me`

### Deploy Your Own

```bash
vercel --prod
```

Vercel automatically optimizes for Farcaster Mini Apps.

---

## Project Structure

```
thumb/
├── contracts/                # Celo-compatible Solidity contracts
├── src/
│   ├── app/                  # Next.js pages + Frame routes
│   ├── components/           # Mini App UI components
│   ├── frames/               # Frames v2 entry points
│   ├── lib/                  # Celo + MiniKit + Farcaster utils
│   ├── config/               # Chain, contract, hub config
├── public/                   # Frame images, metadata, icons
├── hardhat.config.ts
├── README.md
├── package.json
```

---

## How It Works (Waves)

### Wave 1 – Frame Entry + Live Feed
- Frames v2 entry from any cast
- Real-time Celo transaction + social feed
- MiniKit wallet connect

### Wave 2 – AI Insights + Real-Time
- Live event streaming via Celo indexers
- AI summarization (“Top 5 casters just got tipped”)
- Historical data cached on-device

### Wave 3 – Full Mini App + Dev Tools
- Full-screen Mini App experience
- `/nerds` developer dashboard with raw logs
- Anomaly detection + predictions

### Wave 4 – Gamified & Social
- Prediction markets (“Next big tip?”)
- Onchain reactions & leaderboards
- Farcaster notifications via MiniKit

### Wave 5 – Ecosystem Reference
- Open-source SDK for Celo + Farcaster Mini Apps
- Templates & boilerplates
- Deployed as the gold standard for social onchain apps

---

## Why Thumb Accelerates Farcaster + Celo Development

Thumb is built from day one as a **production-grade reference** for the most powerful combo in social crypto today:

**Farcaster + Celo + Mini Apps**

It ships with:
- Perfect cold-start performance in Warpcast
- Battle-tested MiniKit transaction flows
- Real-time feeds that don’t drain battery
- AI insights that feel magical
- One-click deploy pipeline

Fork Thumb. Ship your idea in hours, not weeks.

---

## Roadmap

| Phase       | Focus                              | Status     |
|-------------|------------------------------------|------------|
| Wave 1      | Frame → Live Feed                  | Complete   |
| Wave 2      | AI Summaries + Real-Time           | Complete   |
| Wave 3      | Full Mini App + Dev Dashboard      | Complete   |
| Wave 4      | Predictions + Social Games         | In Progress |
| Wave 5      | SDK Release + Ecosystem Hub        | Next       |

Long-term: Become the Dune + DexScreener for Farcaster social activity.

---

## Contributing

We’re building the future of onchain social. Join us.

```bash
git clone https://github.com/Chidal/thumb.git
git checkout -b feat/your-idea
```

All contributors get:
- Onchain credit
- Early access to SDK
- Shoutouts in Warpcast

---

## License

MIT © 2025 Chidal – Free to fork, ship, and build on.

---

## Acknowledgments

- **Farcaster Team** – For Frames, MiniKit, and the best social layer
- **Celo Team** – For the fastest, most inclusive L1
- **Warpcast** – Where Thumb lives, breathes, and gets thumbed up

---

**Thumb** – Real-time onchain vision, built for Farcaster, powered by Celo.

Open in Warpcast now → **thumb.fcast.me**  
Give it a thumbs up if you like what you see.
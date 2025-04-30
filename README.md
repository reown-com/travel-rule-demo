# Travel Rule Frontend Demo

A Next.js application demonstrating the implementation of the Travel Rule for cryptocurrency withdrawals. This demo showcases how to verify wallet ownership and handle cross-chain transactions while complying with FATF Travel Rule requirements.

## Features

- Multi-chain support (Bitcoin, Ethereum, Solana)
- Wallet connection and ownership verification
- Cross-chain transaction simulation
- Deep linking support for mobile applications
- Travel Rule compliance demonstration

## Tech Stack

- Next.js 14
- TypeScript
- Reown AppKit for wallet connections, SIWX and Travel Rule ownership verification.
- Tailwind CSS for styling
- Shadcn UI components

## Supported Chains

- Bitcoin (Mainnet & Testnet)
- Ethereum (Mainnet)
- Arbitrum
- Solana

## Getting Started

### Prerequisites

- Node.js 18.x or later
- npm or yarn
- A wallet that supports the chains you want to test with

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd travel-rule-frontend
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Create a `.env.local` file in the root directory and add your environment variables:
```env
NEXT_PUBLIC_APPKIT_PROJECT_ID=your_project_id_here
```

4. Start the development server:
```bash
npm run dev
# or
yarn dev
```

The application will be available at `http://localhost:3000`

## Project Structure

```
travel-rule-frontend/
├── app/
│   ├── page.tsx              # Home page
│   ├── withdrawal/
│   │   └── page.tsx          # Withdrawal page
│   └── layout.tsx            # Root layout
├── components/
│   └── ui/                   # UI components
├── context/
│   └── wagmi.tsx             # Wagmi configuration
└── public/                   # Static assets
```

## Usage

1. **Home Page**
   - View available chains
   - Start the withdrawal process

2. **Withdrawal Process**
   - Connect your wallet
   - Verify wallet ownership through message signing
   - Enter withdrawal amount
   - Complete the transaction

3. **Mobile Integration**
   - The application supports deep linking for mobile apps
   - Use the `redirect_uri` parameter to specify your app's scheme

## Chain-Specific Features

### Bitcoin
- Support for both mainnet and testnet
- Custom adapter implementation

### Ethereum
- Mainnet and Arbitrum support
- Ethers adapter integration

### Solana
- Mainnet support
- Solana adapter integration

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Reown AppKit for SIWX and Travel Rule verification.
- Next.js team for the framework
- The open-source community for various dependencies 
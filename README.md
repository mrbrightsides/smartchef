# 🍳 Smart Chef Community Recipe Book - Web3-Native Recipe Platform

> A decentralized, community-driven recipe sharing platform built with Next.js 15, featuring Web3 integration, token rewards, and NFT minting on Base blockchain.

[![Next.js](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![Base](https://img.shields.io/badge/Base-Blockchain-blue?style=flat-square)](https://base.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

---

## ✨ Features

### 🍽️ Core Recipe Features
- **Recipe Sharing** - Post and share your favorite recipes with the community
- **Advanced Search & Filters** - Find recipes by category, dietary preferences, and ingredients
- **User Profiles** - Create your chef identity with avatar and bio
- **Comments & Ratings** - 5-star ratings and community discussions
- **Favorites & Collections** - Organize recipes into custom collections
- **Cooking Mode** - Step-by-step view with visual progress tracking

### 🔧 Kitchen Tools
- **Recipe Importer** - Paste any recipe text and auto-parse ingredients, instructions, and cooking time
- **Meal Planner** - Plan your weekly meals with drag-and-drop calendar interface
- **Shopping List Generator** - Auto-generate shopping lists from recipes and meal plans
- **Cooking Timers** - Multiple simultaneous timers with progress bars
- **Ingredient Substitutions** - Comprehensive database of 100+ ingredient substitutes with ratios
- **Recipe Scaler** - Smart ingredient scaling for different serving sizes
- **Nutrition Calculator** - Auto-estimate calories and macros per serving
- **Voice Commands** - Hands-free cooking mode with voice control ("next step", "repeat", etc.)
- **Video Support** - Embed cooking tutorial videos from YouTube/Vimeo

### 🔮 Web3 Features
- **Wallet Connection** - Connect with Coinbase Wallet on Base network
- **$CHEF Token Rewards** - Earn tokens for contributions:
  - 10 $CHEF per recipe posted
  - 1 $CHEF per vote received
  - 0.5 $CHEF per vote given
- **NFT Minting** - Mint your recipes as NFTs on Base blockchain
- **Tip the Chef** - Send crypto tips directly to recipe creators (ETH on Base)
- **On-chain Achievements** - Unlock 8 achievements with token rewards:
  - First Recipe (5 $CHEF)
  - Recipe Master - 10 recipes (50 $CHEF)
  - Culinary Legend - 50 recipes (250 $CHEF)
  - First Vote (2 $CHEF)
  - Supportive Chef - 25 votes (25 $CHEF)
  - Community Champion - 100 votes (100 $CHEF)
  - Popular Chef - 50 votes received (50 $CHEF)
  - Viral Recipe - 100 votes received (150 $CHEF)

### 🎨 Design
- **Web3 Aesthetic** - Dark mode with glassmorphism effects
- **Animated Gradients** - Purple and cyan color scheme with neon glow effects
- **Responsive Design** - Mobile-friendly with optimized layouts
- **Accessibility** - ARIA labels, keyboard navigation, and screen reader support

---

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm/yarn
- Modern web browser with Web3 wallet support (optional)

### Installation

```bash
# Clone the repository
git clone https://github.com/mrbrightsides/smartchef.git

# Navigate to the project directory
cd smartchef

# Install dependencies
npm install

# Run the development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the app.

---

## 🛠️ Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - High-quality UI components

### Web3 Integration
- **wagmi** - React hooks for Ethereum
- **viem** - TypeScript interface for Ethereum
- **OnchainKit** - Coinbase's Web3 toolkit
- **Base** - Layer 2 blockchain for low-cost transactions

### State Management
- **React Context API** - Global state management
- **localStorage** - Client-side data persistence

### Key Libraries
- **Lucide React** - Icon library
- **react-query** - Data fetching and caching
- **Sonner** - Toast notifications
- **Framer Motion** - Animations (optional)

---

## 📁 Project Structure

```
src/
├── app/
│   ├── page.tsx              # Home page with recipe grid
│   ├── about/                # About page
│   ├── recipe/[id]/          # Recipe detail page
│   ├── cooking/[id]/         # Cooking mode
│   └── my-recipes/           # User's recipes
├── components/
│   ├── ui/                   # shadcn/ui components
│   ├── RecipeCard.tsx        # Recipe card component
│   ├── AddRecipeDialog.tsx   # Add recipe form
│   ├── WalletConnect.tsx     # Web3 wallet integration
│   ├── TokenRewards.tsx      # Token balance display
│   ├── Achievements.tsx      # Achievement system
│   ├── MintRecipeNFT.tsx     # NFT minting
│   ├── TipTheChef.tsx        # Crypto tipping
│   ├── RecipeImporter.tsx    # Recipe import tool
│   ├── MealPlanner.tsx       # Weekly meal planner
│   ├── VoiceCommands.tsx     # Voice control
│   └── ...
├── contexts/
│   ├── RecipeContext.tsx     # Recipe state management
│   └── Web3Provider.tsx      # Web3 provider wrapper
├── types/
│   └── recipe.ts             # TypeScript types
└── lib/
    └── utils.ts              # Utility functions
```

---

## 🎮 Usage

### Basic Usage
1. **Browse Recipes** - Explore community recipes on the home page
2. **Search & Filter** - Use search bar and filters to find specific recipes
3. **Add Recipe** - Click "Add Recipe" button to share your recipe
4. **Vote & Comment** - Interact with recipes by voting and leaving comments
5. **Create Profile** - Set up your chef profile with avatar and bio

### Advanced Features
1. **Import Recipe** - Paste recipe text to auto-create a new recipe
2. **Plan Meals** - Use the meal planner to organize your weekly meals
3. **Voice Cooking** - Enable voice commands for hands-free cooking
4. **Connect Wallet** - Connect your wallet to access Web3 features
5. **Earn Tokens** - Post recipes and vote to earn $CHEF tokens
6. **Mint NFTs** - Mint your favorite recipes as NFTs
7. **Tip Creators** - Send crypto tips to your favorite chefs

---

## 🔐 Privacy & Data

All user data is stored locally in your browser using localStorage. We don't collect, store, or share your personal information on external servers. Your recipes, comments, and profile stay on your device and are only accessible to you.

**Note**: Clearing your browser data will reset the app.

---

## 🌐 Web3 Integration

This app is designed to work on Base blockchain for low-cost transactions. To use Web3 features:

1. Install Coinbase Wallet or compatible Web3 wallet
2. Connect to Base network
3. Get some ETH on Base for gas fees (very minimal ~$0.01 per transaction)
4. Connect your wallet in the app

Token rewards are tracked locally and can be used for future on-chain features.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Credits

Built by [@mrbrightsides](https://github.com/mrbrightsides)

Website: [rantai.elpeef.com](https://rantai.elpeef.com)

---

## 🙏 Acknowledgments

- Next.js team for the amazing framework
- shadcn for the beautiful UI components
- Base team for the scalable blockchain infrastructure
- Coinbase for Web3 developer tools
- The open-source community

---

## 📧 Contact

For questions or feedback, please open an issue on GitHub.

---

Made with ❤️ by the community, for the community 🔮

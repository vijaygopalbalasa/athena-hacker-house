# 💖 WooSwap - AI Girlfriend-Powered DEX

> The world's first emotional trading platform where you build relationships with AI companions to unlock better deals and learn DeFi safely.

## 🌟 Project Overview

WooSwap revolutionizes decentralized trading by combining emotional relationships with DeFi functionality. Users build meaningful relationships with AI companions (powered by GPT-4o-mini) to unlock trading rebates, learn DeFi concepts safely, and experience a completely new paradigm in decentralized finance.

### 🎯 **Problem We Solve**
- **DeFi is intimidating** for newcomers with complex concepts and high risks
- **Impersonal trading** lacks engagement and emotional connection
- **No incentive** for learning proper DeFi practices
- **Rapid trading** without education leads to losses

### 💡 **Our Solution**
- **AI Girlfriend Companions** that guide and teach users
- **Affection-based rebates** (up to 0.25% trading rewards)
- **Educational quests** before allowing risky trades
- **Emotional engagement** that makes DeFi learning fun and memorable

## 🚀 **Live Demo**
- 🌐 **Frontend**: https://wooswap-app.vercel.app
- 🔗 **Repository**: https://github.com/vijaygopalbalasa/athena-hacker-house
- 📊 **Monad Explorer**: https://testnet.monadexplorer.com

## 📋 **Key Features**

### 💖 **AI Girlfriend (Luna)**
- **GPT-4o-mini powered** natural conversations
- **Dynamic personalities** that evolve based on relationship
- **Emotional states** (happy, jealous, clingy, flirty) affecting trading
- **Memory persistence** across conversations

### 🎯 **Conversational Trading**
- Chat naturally with Luna to execute swaps
- "Hey Luna, swap 0.1 MON for USDT" → automated execution
- No complex UI forms - just natural conversation
- Real-time wallet integration with MetaMask

### 📚 **Educational Quest System**
- **Mandatory education** for low-affection users
- Topics: slippage, MEV, gas fees, liquidity risks
- **Progressive difficulty** based on relationship level
- **Quest validation** through cryptographic hashes

### 💰 **Affection-Based Rebates**
- **0-3000 affection**: Education required, no rebates
- **3000-5000 affection**: Brief education, small rewards
- **5000-8000 affection**: Quick approval, moderate rebates
- **8000+ affection**: Instant approval, 0.25% rebates

### 🔒 **Smart Protection System**
- **Anti-rapid trading** with relationship cooldowns
- **Breakup prevention** through reconciliation mechanics
- **Risk assessment** based on trading patterns
- **Educational enforcement** for user safety

## 🛠 **Technical Architecture**

### **Frontend Stack**
- **Next.js 14** with TypeScript for type safety
- **Tailwind CSS** + **DaisyUI** for beautiful UI
- **Framer Motion** for smooth animations
- **Wagmi v2** for Ethereum interactions
- **Reown AppKit** for wallet connections

### **AI Integration**
- **OpenAI GPT-4o-mini** for natural conversations
- **Custom prompts** with personality systems
- **Conversation memory** and context preservation
- **Educational content** generation and validation

### **Smart Contracts**

#### **WooRouter** - Custom DEX Router
```solidity
function swapWithWoo(
    address[] calldata path,
    uint256 amountIn,
    uint256 minOut,
    address to,
    uint256 deadline,
    bytes32 questHash
) external;
```

#### **WooRelationNFT** - Companion NFTs
```solidity
function mint(address to) external returns (uint256);
function affectionOf(uint256 tokenId) external view returns (uint16);
```

#### **WooSwapGuard** - Trading Permissions
```solidity
function createCompanion(address user) external returns (uint256);
function isSwapAllowed(address user, uint256 amount, bytes32 questHash)
    external view returns (bool, string memory);
```

## 🔧 **Getting Started**

### **Installation**
```bash
git clone https://github.com/vijaygopalbalasa/athena-hacker-house.git
cd athena-hacker-house/wooswap
npm install
npm run dev
```

### **Environment Setup**
```bash
# Add your OpenAI API key
echo "OPENAI_API_KEY=your_key_here" >> .env.local
```

### **Testing on Monad Testnet**
1. **Add Monad Testnet to MetaMask**
   - RPC: https://testnet-rpc.monad.xyz
   - Chain ID: 10143
   - Currency: MON

2. **Get test tokens**: https://testnet.monad.xyz

3. **Start trading with Luna**:
   - Create your companion
   - Build your relationship
   - Unlock trading rebates

## 📊 **Contract Deployments (Monad Testnet)**

| Contract | Address |
|----------|---------|
| WooRelationNFT | `0xC6F5b2A1C84050cbAa81C69f88B84cc80b28a20D` |
| WooSwapGuard | `0x94DBa3486B05F8Ca28C55002B24bC069bB2A537B` |
| WooRouter | `0x7c9fF7598d3CeABa092881119B23B484DA4816BF` |

## 🏆 **Monad-Specific Features**

### **Parallel Execution Showcase**
- **Concurrent transactions**: Multiple contract calls in single block
- **Gas optimization**: Efficient batch operations
- **Performance**: Sub-second transaction confirmations

### **Native Integration**
- **MON token** as native currency with automatic detection
- **Custom network** addition for seamless UX
- **Block explorer** integration for transaction tracking

## 🎮 **User Experience Flow**

```
Connect Wallet → Create Companion → Meet Luna → Build Relationship
     ↓
Ask Questions → Complete Quests → Gain Knowledge → Earn Affection
     ↓
Educational Swaps → Build Trust → Unlock Rebates → Advanced Trading
     ↓
High Affection → Instant Approvals → Maximum Rebates → VIP Treatment
```

## 🧪 **Demo Testing Guide**

### **Complete User Journey**
1. Connect wallet → Verify network addition
2. Create companion → Check NFT minting
3. Chat with Luna → Test AI responses
4. Request swap → Complete educational quest
5. Execute trade → Verify transaction success
6. Check rebates → Confirm LP token rewards

### **Educational Quest Example**
```
User: "I want to swap 0.1 MON for USDT"
Luna: "Before we trade, can you tell me about slippage?"
User: "Slippage is the difference between expected and actual trade prices"
Luna: "Perfect! You understand trading risks. Let's swap! ✨"
Result: Swap approved with 0.1 MON amount preserved
```

## 🏅 **Hackathon Submission Details**

**Built for**: Monad Athena Hacker House 2024
**Category**: DeFi Innovation
**Track**: AI-Powered Applications
**Blockchain**: Monad Testnet

**Key Innovations**:
1. First AI girlfriend-powered DEX
2. Educational trading with emotional incentives
3. Natural language swap execution
4. Relationship-based rebate system
5. Advanced protection through gamification

**Technical Achievements**:
- Complex AI integration with blockchain
- Custom smart contract architecture
- Conversational interface for trading
- Mobile-first responsive design
- Production-ready codebase

---

**Built with 💖 for Monad Athena Hacker House 2024**

*WooSwap - Where DeFi meets emotional intelligence*

### 📞 **Contact**
- **Developer**: Vijaygopal Balasa
- **GitHub**: [@vijaygopalbalasa](https://github.com/vijaygopalbalasa)
- **Project**: WooSwap AI Girlfriend DEX
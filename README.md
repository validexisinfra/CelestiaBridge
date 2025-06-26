# 🌉 Celestia Bridge Nodes Registry

This repository serves as a public registry for **Celestia Bridge Node operators**, allowing validators to associate their:

- ✅ **Bridge Node Peer ID**
- ✅ **On-chain validator address**
- ✅ **Additional metadata** (logo, socials, Keybase, etc.)

with their **validator identity**.

> 🛰️ Data submitted here is used by [https://celestiabridge.com](https://celestiabridge.com) and other tools in the ecosystem to **verify** and **display** bridge node operators.

---

## 🛠 How to Register Your Bridge Node

Follow these simple steps to get listed:

### 1. Fork this repository  
Click the **Fork** button in the top-right of the page.

### 2. Create your metadata file  
Navigate to the `CelestiaBridge/` directory in your fork.  
Create a new file named `<your_validator_or_keybase_id>.json`  
_(e.g., `validexis.json`)_

### 3. Use the following format:

#### JSON format

```
{
  "keybaseIdentity": "YOUR_KEYBASE_ID",
  "name": "Your Validator Name",
  "website": "https://yourwebsite.example",
  "email": "youremail@example.com",
  "validatorAddress": "celestiavaloper1youraddress...",
  "bridgeNodeID": "12D3KooWyourpeerid...",
  "logo": "https://yourwebsite.example/logo.png",
  "telegram": "yourtelegramhandle",
  "twitter": "yourtwitterhandle",
  "github": "yourgithubhandle",
  "description": "Validator and infra provider for Celestia and other Cosmos-based networks"
}
```

> 📌 **Note:** Please use **direct URLs** to PNG or SVG logos.  

---

## 🔍 How to Find Your Bridge Node Peer ID

Run this command on your Celestia bridge node:

#### 🧪 For **Testnet (mocha-4)**:

```bash
celestia p2p info --node.store ~/.celestia-bridge-mocha-4/
```

#### 🌐 For **Mainnet**:

```bash
celestia p2p info --node.store ~/.celestia-bridge/
```

Copy the **Peer ID** from the output and paste it into the `bridgeNodeID` field of your JSON file.

---

## 📤 Submission Process

1. Commit your `.json` file to your fork  
2. Open a **Pull Request (PR)** to this repository  
3. Once reviewed and merged, your metadata will be picked up automatically by [https://celestiabridge.com](https://celestiabridge.com) and similar tools

---

## 📬 Contact

If you have any questions or need help:

- Telegram: [@validexis](https://t.me/validexis)
- GitHub: [https://github.com/validexisinfra](https://github.com/validexisinfra)


# 🟣 Rialo Stake-for-Service Playground

An interactive **frontend-only simulation** demonstrating how **staking rewards can autonomously pay for on-chain services** — based entirely on the Rialo **Stake-for-Service** (SfS) model.

This playground visually teaches the core mechanism from the official Rialo blog:

➡ Stake RLO
➡ Earn Rewards
➡ A Routing Fraction sends part into the **ServicePaymaster (SPM)**
➡ SPM **mints service credits**
➡ Credits **pay for continuous service usage**

📌 **Zero wallet required**
📌 **Zero blockchain dependency**
📌 **Purely educational, UX-driven simulation**

---

## 🎯 Purpose

To make Stake-for-Service **easy to understand** through:

* Real-time feedback
* Interactive sliders & inputs
* Visual economic flow
* Architecture & formula explanation

Users learn by testing:

> How much RLO to stake
> How much yield to route (φₚ)
> Whether the service can sustain itself

---

## 🧠 What Stake-for-Service Solves

> Apps should run **even when users have empty wallets**

This model uses staking yield to **fund execution** automatically, improving:

✔ User onboarding
✔ Predictable operational budgets
✔ Long-term service sustainability

---

## ✨ Features

| Feature                      | Description                          |
| ---------------------------- | ------------------------------------ |
| Stake input                  | User sets how much RLO is staked     |
| Routing Fraction slider (φₚ) | Set what % of rewards become credits |
| Live Service Status          | Running / Low Credits / Stopped      |
| SPM Credit Balance           | Credits minted from routing          |
| Wallet Rewards               | Liquid rewards not routed            |
| Credits vs Time Graph        | Shows sustainability over epochs     |
| Allocation Donut Chart       | Visual split of rewards              |
| Architecture Diagram         | Blog-aligned SfS flow                |
| Official Formula             | Shown & explained interactively      |
| Tooltips Everywhere          | Glossary from the blog               |

---

## 🧮 Official SfS Formula (From Rialo Blog)

[
R^{(svc)}*{t+1} = \sum*{p \in S_t} \phi_p \cdot r_p(t+1)
]

Where:

* ( \phi_p ) = Routing Fraction
* ( r_p(t+1) ) = Reward earned next epoch
* ( R^{(svc)} ) = Total routed into ServicePaymaster

> “A portion of rewards is routed each epoch to pay for services.”
> — *Rialo: Stake-for-Service blog*

---

## 🧩 Architecture Included

```
SfS Position
     ↓
Staking Rewards
     ↓
Routing Fraction φₚ
     ↓
+───────────────+──────────────+
| Liquid Rewards| Service Credits|
|  (Wallet)     |   (SPM)       |
+───────────────+──────────────+
                     ↓
              Service Usage
```

---

## 🖌️ Design System

🎨 Brand Colors

* Mint → `#A9DDD3`
* Soft Beige → `#E8E3D5`
* Deep Black → `#010101`

💎 Style

* Rounded playground UI
* Subtle mint animations
* Modern clean typography (DM Sans)

---

## 🛠️ Tech Stack

| Layer      | Choice                          |
| ---------- | ------------------------------- |
| UI         | HTML + Tailwind CSS             |
| Charts     | Chart.js                        |
| Logic      | Pure JavaScript (No blockchain) |
| Deployment | Works anywhere — static hosting |

---

## 🧩 How to Run Locally

```bash
git clone <your-repo-url>
cd your-repo-folder
open index.html
```

(or drag `index.html` into your browser)

---

## 📌 Disclaimer

This is an **educational simulation**.
It does **not** represent real staking or smart-contract behavior — only the **mechanics explained in the blog**.

---

## 🤝 Credits

Created by **Aman**
Inspired by:
🔗 [https://www.rialo.io/posts/stake-for-service](https://www.rialo.io/posts/stake-for-service)

If you found this useful — star ⭐ the repo!

---

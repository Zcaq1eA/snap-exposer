# 🕵️‍♂️ Snap Exposer

A research-driven repository dedicated to analyzing and exposing security risks in [MetaMask Snaps](https://metamask.io/snaps/), with a strong focus on recon, vulnerable dependencies, and bug bounty reporting.

## 🔍 What is Snap Exposer?

Snap Exposer is a security research project aimed at:

- Identifying vulnerable or outdated dependencies in MetaMask Snap packages
- Mapping dependency chains that may introduce risk
- Testing real-world Snaps (e.g. `solflare-snap`, `@leapwallet/metamask-cosmos-snap`)
- Documenting attack surfaces for ethical hacking and responsible disclosure

## 🚀 Project Goals

- ✅ Perform reconnaissance on all Snap packages in MetaMask’s bug bounty scope
- ✅ Analyze dependency trees and detect known CVEs
- ✅ Brute-force testing Snap endpoints using tools like Burp Suite & FFUF
- ✅ Build a portfolio of valid, high-quality reports on HackerOne

## 🛠️ Tools Used

| Tool             | Purpose                          |
|------------------|----------------------------------|
| Burp Suite       | Web proxy for testing interactions |
| Nmap             | Network scanning & port detection |
| FFUF             | Fuzzing hidden routes             |
| GAU & Waybackurls| Historical URL gathering          |
| SQLMap           | SQL injection testing             |
| Katana           | Web crawler for recon             |
| Sublist3r        | Subdomain enumeration             |
| curl             | Manual testing & scripting        |

## 🧪 Example Targets

- [`@leapwallet/metamask-cosmos-snap`](https://www.npmjs.com/package/@leapwallet/metamask-cosmos-snap)
- [`solflare-snap`](https://www.npmjs.com/package/solflare-snap)
- [`@leapwallet/buffer-boba`](https://www.npmjs.com/package/@leapwallet/buffer-boba)

## 📂 Repo Structure

snap-exposer/
├── reports/ # PDF or markdown-based vulnerability reports
├── tools/ # Scripts, recon tools, helpers
├── findings/ # Raw vulnerability data and dependency graphs
├── screenshots/ # Evidence from Burp or browser testing
└── README.md # This file


## 🧠 Who Am I?

My name is **Awirut Pukoed**, a professional bug bounty hunter from Thailand 🇹🇭. I specialize in:

- Reconnaissance
- Web vulnerability testing
- Python scripting
- Deep analysis of Web3 and Snap ecosystems

## 🛡️ Disclaimer

This project is for **educational and ethical research purposes only**. I do not support or condone any illegal activity. All disclosed vulnerabilities will follow responsible disclosure policies and be reported via [HackerOne](https://hackerone.com/).

---

**Let’s expose insecure Snaps—one bug at a time. 🔓**

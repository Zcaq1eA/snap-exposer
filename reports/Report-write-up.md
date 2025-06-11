# 🐞 Bug Report: SSRF via Vulnerable Axios in @leapwallet/metamask-cosmos-snap

## 📌 Scope
- **Target Snap ID**: `npm:@leapwallet/metamask-cosmos-snap`
- **Program**: MetaMask Bug Bounty
- **Environment**: Public Snap distributed via NPM

---

## 🔍 Summary
The `@leapwallet/metamask-cosmos-snap` package includes a vulnerable version of Axios (`<=0.29.0`) which is known to be susceptible to **Server-Side Request Forgery (SSRF)** and **Cross-Site Request Forgery (CSRF)**. This can potentially allow attackers to craft malicious Snap transactions that abuse underlying Axios behavior to perform unauthorized internal requests or leak sensitive data.

---

## ✅ Vulnerability Type
- [x] SSRF (Server-Side Request Forgery)
- [x] CSRF (Cross-Site Request Forgery)
- [ ] Misconfigured Snap Permissions

---

## 🚦Severity
- **OWASP Rating**: High
- **Impact**: Axios v0.29.0 is known for security issues including improper request handling, which may allow attackers to:
  - Reach internal resources
  - Leak user IPs or system data
  - Forge requests in a Snap context

---

## 🧪 Proof of Concept (PoC)

### Dependency Chain:
@leapwallet/metamask-cosmos-snap

└── @leapwallet/buffer-boba

└── stridejs

└── osmojs

└── @osmonauts/helpers

└── axios@0.27.2

## 📃References
[CWE-918: Server-Side Request Forgery (SSRF)](https://cwe.mitre.org/data/definitions/918.html)
[OWASP A10 SSRF (2021)](https://owasp.org/Top10/A10_2021-Server-Side_Request_Forgery_%28SSRF%29/)
[OWASP SSRF Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet.html)
CVE‑2022‑28168 – Axios SSRF advisory


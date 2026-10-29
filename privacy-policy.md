# Privacy Policy for PolyWatcher

**Effective date:** October 29, 2026  
**Publisher:** K&BOTS STUDIO  
**Product:** PolyWatcher (Chrome extension)

This Privacy Policy describes how PolyWatcher (“the Extension,” “we,” “us”) handles information when you install and use the Extension. By using the Extension, you agree to this Policy.

> **Contact:** For privacy questions, email **`18817532236+privacy@mail.grokbot.com`** 

---

## 1. What PolyWatcher is

PolyWatcher shows **1-day-delayed, category Top3 wallet rankings** derived from **public Polymarket market data**, as an overlay while you browse `polymarket.com`, and in the Extension popup.  

PolyWatcher is **not** affiliated with Polymarket. It is **not** a trading bot, copy-trading tool, or brokerage.

**Important:** Ranking and market data are for **reference only**. They are **not** financial, investment, tax, or legal advice, and they do **not** guarantee any profit if you follow any wallet, ranking, or signal.

---

## 2. Information we do **not** collect

We do **not**:

- Ask for, collect, or store your Polymarket (or any other) **account password**, private keys, seed phrases, or wallet secrets  
- Access your Polymarket login session for the purpose of signing in as you  
- Sell your personal information  
- Run third-party advertising SDKs, ad trackers, or cross-site advertising cookies inside the Extension  
- Require you to create a PolyWatcher account to use the free rankings overlay

---

## 3. Information the Extension uses

### 3.1 Data stored only on your device (`chrome.storage.local`)

The Extension may store locally on your browser:

| Item | Purpose |
|------|---------|
| Cached ranking JSON | Faster display; reduce repeated network fetches |
| Cache timestamp / API base used for that cache | Freshness and correctness of cache |
| UI preference (e.g. panel collapsed/hidden) | Remember how you like the on-page panel |
| Optional developer API override (hidden debug UI only) | Let maintainers point at a different rankings endpoint during testing |

This local data stays in your Chrome profile unless you clear Extension data or uninstall.

### 3.2 Background refresh (`chrome.alarms`)

The Extension uses Chrome **alarms** (about every 30 minutes) to refresh the rankings cache in the background so the panel stays reasonably up to date.

### 3.3 Network requests to our rankings API

To show rankings, the Extension’s background script requests ranking snapshots (JSON) from a **publisher-operated HTTPS rankings API** (for store builds this is currently `https://api.logic.red`).  

That request is a normal HTTPS call. Like most websites and APIs, **our server may automatically receive technical request metadata**, such as:

- IP address  
- date/time  
- User-Agent / browser type  
- requested URL/path  

We use this only to operate, secure, and debug the rankings service (for example, abuse prevention and uptime). We do **not** use it to build advertising profiles.

**We do not need you to send your Polymarket password for this fetch.** The payload is public ranking-style data for the free tier.

### 3.4 Content script on `polymarket.com`

On `https://polymarket.com/*` (and `www`), the Extension injects a **UI panel** (and related styles) to display rankings and links to public Polymarket profile pages (e.g. `/profile/<wallet>`).  

The content script is for **display and Extension messaging**. It is **not** designed to harvest your password or payment details from Polymarket forms.

### 3.5 Permissions (Chrome)

Typical store permissions and why:

- **`storage`** — local cache and UI preferences (see §3.1)  
- **`alarms`** — periodic cache refresh (see §3.2)  
- **Host access to Polymarket** — inject the on-page panel (see §3.4)  
- **Host access to our rankings API origin** — fetch ranking JSON (see §3.3)

---

## 4. How we use information

We use the information in §3 only to:

- Provide and refresh rankings in the Extension  
- Remember your local UI preferences  
- Operate, secure, and troubleshoot the rankings API  

We do **not** sell personal information. We do **not** use Extension data for third-party advertising.

---

## 5. Sharing

We do not sell your personal information.  

We may disclose information if required by law, to protect rights and safety, or to service providers who help us run infrastructure **only as needed to operate the rankings API** (for example, a hosting provider that processes standard server logs). Those parties are not authorized to use the information for their own marketing.

Public ranking content shown in the Extension comes from public market data ecosystems (including Polymarket’s public surfaces/APIs as processed by our collector). Your use of Polymarket itself remains subject to **Polymarket’s** own terms and privacy policy.

---

## 6. Data retention

- **On your device:** local cache and preferences remain until you clear site/extension data, reset the Extension, or uninstall.  
- **On our rankings API:** routine server logs are kept only as long as reasonably needed for security and operations, then discarded or rotated under normal hosting practice. We do not build long-term advertising profiles from Extension use.

---

## 7. Children’s privacy

The Extension is not directed at children under 13 (or the equivalent minimum age in your jurisdiction). We do not knowingly collect personal information from children.

---

## 8. International users

If you use the Extension from outside the country where our infrastructure is hosted, your technical request metadata (see §3.3) may be processed in the region where the API is hosted.

---

## 9. Changes

We may update this Policy from time to time. The “Effective date” at the top will change when we do. Continued use of the Extension after an update means you accept the revised Policy.

---

## 10. Contact

Privacy questions: **`18817532236+privacy@mail.grokbot.com`**  
Publisher: **K&BOTS STUDIO**  
Product: **PolyWatcher**

---

## Disclaimer (product)

PolyWatcher provides delayed public-market ranking data for **reference only**. Nothing in the Extension is an offer to buy or sell any asset, a recommendation of any wallet or market, or a promise of profit. You are solely responsible for your own decisions.

---

# 隐私政策（中文摘要）

**生效日期：** 2026年10月29日  
**发布者：** K&BOTS STUDIO  
**产品：** PolyWatcher（Chrome 扩展）

本摘要便于中文读者快速了解；**如与上方英文正文不一致，以英文正文为准。**

### 我们做什么
在浏览 `polymarket.com` 时显示面板，并在扩展弹窗中展示基于公开市场数据整理的、**约延迟 1 天**的分类 Top3 钱包排行。数据**仅供参考**，**不构成**投资、理财、税务或法律建议，**不保证**跟单或按排行操作可以盈利。与 Polymarket **无隶属关系**。

### 我们不做什么
- 不收集、不索取 Polymarket（或其他）**账号密码**、私钥、助记词  
- 不出售用户个人数据  
- 不在扩展内接入第三方广告追踪 SDK  

### 本地与网络
- 使用 `chrome.storage.local` 在**本机**缓存排行 JSON 与界面偏好（如面板折叠）  
- 使用 `chrome.alarms` **约每 30 分钟**后台刷新缓存  
- 后台向我们运营的**排行 HTTPS API** 拉取公开排行 JSON；服务器可能留下常规访问日志（如 IP、时间、User-Agent），仅用于运维与安全，不做广告画像  
- 在 `polymarket.com` 注入展示用面板，用于显示排行与跳转公开主页链接  

### 联系
隐私相关问题请发邮件至 **`18817532236+privacy@mail.grokbot.com`**。


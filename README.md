# Awesome-Online-Community-Forum-Software

# Awesome Online Community & Forum Software

> A curated list of top Online Community and Forum Software platforms — both SaaS/Hosted commercial solutions and open-source alternatives for building discussion forums, member communities, and knowledge-sharing spaces.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [Open-Source Software](#-open-source-software)
  - [Discourse](#discourse)
  - [Flarum](#flarum)
  - [NodeBB](#nodebb)
  - [Apache Answer](#apache-answer)
  - [phpBB](#phpbb)
  - [MyBB](#mybb)
  - [Simple Machines Forum](#simple-machines-forum)

---

## 📈 Sector Overview & Market Dynamics

The global online community and forum platform market is estimated at between **$800M and over $6B** (projected to reach $10B+ by the early 2030s at a 10%–15% CAGR), depending on whether enterprise social networks are included. The sector is **moderately to highly fragmented** among modern creator and brand-led SaaS tools and open-source alternatives, though heavily concentrated at the top enterprise level where large social and customer engagement suites dominate.

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Online Community and Forum Software platforms. These are not open-source but are included as reference points for feature comparison. Sorted in descending order by company scale (annual revenue / valuation).

| Platform | Company Scale (Revenue / Valuation) | Pricing (Starting Tier) | Free Tier / Trial Limits | Key Features & Positioning |
|---|---|---|---|---|
| **Khoros Communities** | ~$280M+ ARR (Vista Equity Partners-backed) | Custom enterprise quote (starts ~$160,000/year; implementation ~$10k–$75k+) | No permanent free plan; No free trial available (sales demo only) | Enterprise-scale community forums, ideation, knowledge base, and social media management for massive global brands. |
| **Higher Logic Vanilla** | ~$68M ARR ($55M growth funding from JMI Equity) | Custom enterprise quote (starts ~$24,000/year or ~$599/month for up to 1,000 users) | No permanent free plan; No public free trial (guided sales demo only) | Enterprise community bundle with multi-forum architecture, advanced SSO, deep CRM/helpdesk integrations, and SLAs. |
| **Circle** | ~$68M ARR ($200M–$250M valuation) | $89/month (Professional plan, billed annually) | No permanent free plan; 14-day free trial (includes core features; no credit card required) | All-in-one creator and modern brand community with courses, live events, paywalls, and group discussions. |
| **Mighty Networks** | ~$8M–$38M ARR ($200M–$250M valuation) | $79/month (Launch Plan, billed annually; 2% transaction fee) | No permanent free plan; 14-day free trial (access to Launch/Course features; no credit card required) | Creator- and educator-focused community with built-in native courses, iOS/Android apps, livestreams, and memberships. |
| **Bettermode** | ~$3.1M ARR ($7.5M total venture funding) | $149/month (Starter plan, billed annually; up to 10k members) | No permanent free plan; 14-day free trial (access to Starter/Growth features; no credit card required) | Highly customizable customer community platform with AI search, modular layout builder, and CRM integrations. |
| **Invision Community** | ~$1.8M ARR (Bootstrapped / privately held) | $89/month (Creator plan, billed annually) | No permanent free plan; 14-day free trial (limited to temporary subdomain, outbound email disabled, no marketplace plugins; no credit card required) | Feature-rich forum and community platform with courses, live topics, calendar events, and granular content moderation. |

---

## 🟩 Open-Source Software

Self-hosted, community-driven Online Community and Forum Software tools. The open-source ecosystem spans **mature enterprise-grade platforms**, **lightweight modern forums**, **real-time Node.js forums**, and **Apache-governed Q&A systems**.

### Discourse
**Stack:** Ruby on Rails / PostgreSQL / Redis | **License:** GPL-2.0
Discourse is the industry standard for self-hosted forums, used by Docker, Figma, Mozilla, and the Rust community [citation:2][citation:15]. It offers **threaded discussions, trust levels, automated moderation, rich notifications, and a plugin ecosystem** covering chat, polls, gamification, and more. Built-in features include full-text search, SSO (SAML, OIDC, LDAP, social login), Akismet anti-spam integration, and email-in (reply to threads via email) [citation:2]. **Resource requirements:** 2 GB RAM minimum, 4 GB recommended, with 2+ CPU cores and 10 GB+ disk [citation:2]. SMTP is mandatory—Discourse cannot function without email. **Caveats:** Uses a custom launcher rather than standard Docker Compose, and Ruby on Rails can be slow without adequate resources [citation:2].
**Best for:** Established communities, product support forums, and organizations needing robust moderation, SSO, and a mature plugin ecosystem, accepting the higher resource requirements.

### Flarum
**Stack:** PHP / MySQL | **License:** MIT
Flarum is a modern, lightweight forum built with PHP and Mithril.js, described as "the antithesis of Discourse's feature density" [citation:2]. It offers a **fast, responsive UI, low resource requirements (512 MB RAM), and a clean, modern design** with Markdown support and a growing extension ecosystem [citation:2][citation:3]. It has **16,238 GitHub stars** and is actively maintained [citation:3]. **Trade-offs:** Fewer features than Discourse out of the box, a smaller community and extension library, no built-in chat, and less mature moderation tools [citation:2].
**Best for:** Small to medium communities wanting a clean, modern forum without the overhead of Discourse—great for hobby communities, project forums, and small organizations.

### NodeBB
**Stack:** Node.js / MongoDB or Redis | **License:** GPL-3.0
NodeBB is a Node.js forum with **real-time updates via WebSocket/Socket.io**—posts appear instantly without page refreshes, and notifications pop up in real-time [citation:2][citation:15]. It offers **threaded and flat topic views, social-style notifications, presence indicators, reputation/karma, and a plugin system** with 100+ modules [citation:15]. It supports MongoDB, PostgreSQL, or Redis, with social login (Google, Facebook, GitHub) and solid REST/WebSocket APIs [citation:2]. **Trade-offs:** Fewer plugins than Discourse, MongoDB dependency adds operational complexity, and the UI feels less polished [citation:2][citation:15]. A hosted Starter plan is **$20/month** with 50,000 pageviews and 5 GB storage [citation:13].
**Best for:** Communities where real-time is core to the experience (gaming, tech, live discussions) and the team already works with Node.js.

### Apache Answer
**Stack:** Go / React / Docker | **License:** Apache-2.0
Apache Answer is an Apache-governed **Q&A platform** for teams of any scale, suitable for community forums, help centers, or knowledge management [citation:3]. It runs via a single Docker command and provides a plugin system for extending features. It is positioned as a lightweight, Apache-licensed alternative to proprietary Q&A platforms.
**Best for:** Teams wanting a focused Q&A platform under a permissive Apache-2.0 license with simple Docker deployment, particularly in the Apache ecosystem.

### phpBB
**Stack:** PHP / MySQL/MariaDB/PostgreSQL/SQLite | **License:** GPL-2.0
phpBB is the most widely deployed open-source forum platform, with a long history and massive community [citation:14]. It provides flat forums, user-selectable themes, WYSIWYG editor, LDAP and OAuth SSO, and full export/portability. It has an extensive extension and style ecosystem. **Trade-off:** The interface feels dated compared to modern platforms like Discourse and Flarum, and performance can degrade at scale without optimization.
**Best for:** Communities wanting a proven, battle-tested forum with a massive ecosystem and low hosting requirements, accepting a dated UI.

### MyBB
**Stack:** PHP / MySQL | **License:** LGPL
MyBB is a free, open-source forum platform with a focus on ease of use and extensibility [citation:14]. It provides flat and threaded discussions, user-selectable themes, WYSIWYG editor, and SSO support. It is positioned for communities wanting a straightforward forum with a gentler learning curve than phpBB.
**Best for:** Communities wanting an accessible, LGPL-licensed forum with a straightforward setup, accepting a smaller ecosystem than the largest platforms.

### Simple Machines Forum
**Stack:** PHP / MySQL/MariaDB/PostgreSQL | **License:** BSD
Simple Machines Forum (SMF) is a free, professional-grade forum package for setting up online communities, with active maintenance (updated August 2026) [citation:14]. It provides flat forums, threaded discussions, WYSIWYG editor, and SSO support. It is positioned as a straightforward, BSD-licensed alternative to phpBB.
**Best for:** Communities wanting a permissive BSD-licensed forum with active maintenance, accepting a smaller ecosystem than phpBB.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Real-Time | SSO | Self-Hosted | Best For |
|----------|---------|-------|-----------|-----|-------------|----------|
| **Bettermode** | Proprietary | Cloud | (Check) | ✅ | ❌ | Modern community + AI |
| **Circle** | Proprietary | Cloud | ✅ Live rooms | ✅ Custom (Plus) | ❌ | Creator community + payments |
| **Mighty Networks** | Proprietary | Cloud | ✅ Chat | (Check) | ❌ | Creator community + native apps |
| **Higher Logic Vanilla** | Proprietary | Cloud | ❌ | ✅ SAML/OAuth | ❌ | Enterprise community |
| **Khoros** | Proprietary | Cloud | ❌ | ✅ | ❌ | Large brand communities |
| **Invision Community** | Proprietary | Cloud | ✅ Live topics | ✅ | ❌ | Full-featured community |
| **Discourse** | GPL-2.0 | Ruby/Rails | Polling | ✅ SAML/OIDC/LDAP | ✅ | Proven enterprise forum |
| **Flarum** | MIT | PHP/MySQL | Polling | Via extension | ✅ | Lightweight modern forum |
| **NodeBB** | GPL-3.0 | Node.js | ✅ WebSocket | ✅ Social login | ✅ | Real-time Node.js forum |
| **Apache Answer** | Apache-2.0 | Go/React | (Check) | (Check) | ✅ | Apache Q&A platform |
| **phpBB** | GPL-2.0 | PHP/DB | ❌ | ✅ LDAP/OAuth | ✅ | Proven legacy forum |
| **MyBB** | LGPL | PHP/MySQL | ❌ | ✅ | ✅ | Accessible legacy forum |
| **SMF** | BSD | PHP/DB | ❌ | ✅ | ✅ | Permissive BSD forum |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Online Community or Forum Software tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The forum landscape splits between **Discourse** (the mature, feature-dense standard with 200+ plugins and enterprise SSO) and **lighter modern alternatives** (Flarum for clean PHP-based forums, NodeBB for real-time WebSocket discussions) [citation:2][citation:15]. **Discourse** remains the dominant choice for serious communities with hundreds or thousands of daily posters, requiring 2-4 GB RAM but delivering trust levels, built-in chat, and battle-tested moderation [citation:2]. **Flarum** is the best fit for small to medium communities wanting a modern UI on modest hardware (512 MB RAM) [citation:2]. **NodeBB** excels where real-time interaction is core, using WebSockets for instant updates [citation:15]. Legacy platforms like phpBB and SMF remain viable for communities valuing stability and low hosting costs over modern UI. Commercial platforms like Bettermode and Circle offer polished experiences with AI and payments built in, at **$89-149/month** [citation:6][citation:7].

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐

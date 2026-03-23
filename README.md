

<div align="center">

![RuneForge ModKeeper Banner](https://raw.githubusercontent.com/MelancholySlime/RuneForge-ModKeeper/main/banner.png)

#  RuneForge ModKeeper

[![Auto Scraper](https://github.com/MelancholySlime/RuneForge-ModKeeper/actions/workflows/runeforge_scraper.yml/badge.svg)](https://github.com/MelancholySlime/RuneForge-ModKeeper/actions/workflows/runeforge_scraper.yml)
[![Last Commit](https://img.shields.io/github/last-commit/MelancholySlime/RuneForge-ModKeeper?color=7c3aed&label=Last%20Update&logo=github)](https://github.com/MelancholySlime/RuneForge-ModKeeper/commits/main)
[![Repo Size](https://img.shields.io/github/repo-size/MelancholySlime/RuneForge-ModKeeper?color=db2777&label=Archive%20Size&logo=databricks)](https://github.com/MelancholySlime/RuneForge-ModKeeper)
[![Source](https://img.shields.io/badge/Source-Runeforge.dev-f59e0b?logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0xMiAyTDIgN2wxMCA1IDEwLTV6TTIgMTdsOCA0IDgtNE0yIDEybDggNCA4LTQiLz48L3N2Zz4=)](https://runeforge.dev)
[![League of Legends](https://img.shields.io/badge/Game-League%20of%20Legends-C89B3C?logo=riot-games)](https://leagueoflegends.com)

*An automated archive that collects, preserves, and loves every single mod from [Runeforge.dev](https://runeforge.dev) — every version, every artifact, without exception.*

</div>
<div align="center">

🌐 **Language / Ngôn ngữ:** [🇬🇧 English](./README.md) · [🇻🇳 Tiếng Việt](./README.vi.md)

</div>

---

## 📖 About

**RuneForge ModKeeper** is a fully automated archival system that runs daily at **7:00 AM (UTC+7)** — silently fetching and preserving every `.fantome` mod file published on [Runeforge.dev](https://runeforge.dev): custom skins, sound effects, VFX, loading screens, and more for **League of Legends**.

No mod goes forgotten. No version gets left behind.

---

## 📦 Repository Structure

Files are organized by `Part` directories, each holding up to **~990 mod folders**. When a Part fills up, a new one is automatically created.

```
📦 RuneForge-ModKeeper/
├── 📁 Part1/
│   ├── 📂 Demon Yasuo LOLSKINARCHIVE/
│   │   └── demon-yasuo-lolskinarchive-v2.fantome
│   └── 📂 Spirit Blossom Yone Chroma VFX/
│       ├── spirit-blossom-yone-chroma-vfx_1.0.0.fantome
│       └── spirit-blossom-yone-chroma-vfx_1.1.0.fantome
├── 📁 Part2/ ...
└── 📁 PartN/ ...
```

> Files larger than **50 MB** are uploaded directly to [GitHub Releases](https://github.com/MelancholySlime/RuneForge-ModKeeper/releases) instead of commits.

---

## ⚙️ How It Works

```
Runeforge.dev ──────► Scraper Bot ──────► GitHub Repository
  (2,800+ mods)       (Daily 7AM)            (This archive)
```

| Step | Action |
|------|--------|
| 🔍 **Scan** | Crawl all 2,800+ mod posts across 120 pages |
| 📋 **Compare** | Cross-reference with `_runeforge_scraped.json` history |
| ☁️ **Cloud Check** | Query GitHub API Tree — skip files already in the cloud |
| 📥 **Download** | Fetch ALL artifacts of ALL versions |
| 📤 **Push** | Auto-push every ~950 MB to stay within GitHub limits |

---

## 📊 Archive Statistics

| Metric | Value |
|--------|-------|
| 🌐 Source | [runeforge.dev](https://runeforge.dev) |
| 🎮 Total Mods Tracked | 2,800+ |
| 🗓️ Archive Created | March 12, 2026 |
| 🔄 Update Frequency | Daily · 7:00 AM UTC+7 |
| 💾 Archive Size | ~34 GB and growing |
| 📦 Max Files per Part | 990 |
| 🚀 Max Batch per Push | 999 MB |

---

## 🔗 Related Links

| Link | Description |
|------|-------------|
| 🌐 [Runeforge.dev](https://runeforge.dev) | Original mod hosting platform |
| 🛠️ [cslol-manager](https://github.com/LeagueToolkit/cslol-manager) | Tool to apply `.fantome` mods in-game |
| 📋 [Action Logs](https://github.com/MelancholySlime/RuneForge-ModKeeper/actions) | Live scraper run history |

---

## 💌 A Note to Mod Authors

This archive was built with love and deep respect for the creative community. We do **not** claim ownership of any mod here — all credit belongs to the original creators on Runeforge.

**If you are a mod author and wish to have your work removed**, please open an [Issue](https://github.com/MelancholySlime/RuneForge-ModKeeper/issues) with the subject `[Takedown Request]`. Your request will be honored promptly and with care. 🌷

---

<div align="center">
  <sub>Maintained with ☕ and 💖 · Automated by GitHub Actions · Not affiliated with Riot Games</sub>
</div>

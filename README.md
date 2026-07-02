# 🛰️ OpentheDoor

A single-file, interactive learning platform for **Nmap** — the network mapper. Built as a searchable field manual you can open in any browser, no build step, no dependencies, no backend.

![type](https://img.shields.io/badge/type-single--file%20HTML-00d9ff)
![deps](https://img.shields.io/badge/dependencies-none-00e676)
![license](https://img.shields.io/badge/license-MIT-b34bff)

## ✨ Live Preview

Just open [`nmap-field-manual.html`](./nmap-field-manual.html) in any modern browser — that's the whole app.

## 📚 What's Inside

| Section | Description |
|---|---|
| **What Is Nmap?** | The four core scan phases — host discovery, port scanning, version detection, and NSE scripting |
| **Installation** | Copy-paste install commands for Debian/Ubuntu, Fedora/RHEL, macOS, Windows, and Kali |
| **Command Anatomy** | Breakdown of target specification, port specification, timing, and output flags |
| **Scan Console** | A searchable, filterable database of 35+ flags and options — scan types, host discovery, detection, and evasion — tagged by root requirement and network "footprint" |
| **NSE Script Engine** | All 14 Nmap Scripting Engine categories explained (`safe`, `vuln`, `exploit`, `brute`, etc.) |
| **Timing Templates** | Interactive breakdown of `-T0` through `-T5`, when to use each |
| **Firewall/IDS Evasion** | 8 evasion techniques (fragmentation, decoys, spoofing, idle scan, and more) |
| **Legal & Ethics** | A clickable pre-engagement checklist — get authorization before you scan anything |
| **Cheat Grid** | 16 ready-to-use one-liner commands for quick reference |

## 🚀 Usage

No installation required.

```bash
git clone https://github.com/<your-username>/nmap-field-manual.git
cd nmap-field-manual
open nmap-field-manual.html   # or just double-click it
```

Or use GitHub Pages to host it live — see [Deploying with GitHub Pages](#-deploying-with-github-pages) below.

## 🌐 Deploying with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder.
4. Save — your manual will be live at `https://<your-username>.github.io/<repo-name>/nmap-field-manual.html`.

> Tip: rename the file to `index.html` if you want it to load at the root of your Pages URL.

## 🛠️ Tech

- Pure HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, no npm install.
- Fonts loaded from Google Fonts (Space Grotesk, Inter, JetBrains Mono).
- Fully self-contained: works offline once the fonts are cached, and all data lives inline in the file.

## ⚠️ Disclaimer

This project is an educational reference. Nmap is a powerful network scanning tool — **only scan systems you own or have explicit, written authorization to test.** Unauthorized scanning may be illegal in your jurisdiction even without causing damage. See the Legal & Ethics section in the manual before running any scan technique described here.

## 🤝 Contributing

Found an outdated flag, a missing NSE category, or a typo? PRs welcome. All content lives inline in `<script>` data arrays inside the HTML file — search for `scanData`, `nseData`, `timingData`, `evasionData`, or `cheatCommands` to find what you're looking for.

## 📄 License

MIT — see [LICENSE](./LICENSE) for details.

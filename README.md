# 🦉 OIndex

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-ORecon%20%2F%20OSINT-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Python-3.x-blue?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OIndex** is a Google Dork builder and OSINT search tool — browse 50+ built-in templates across 8 categories, build custom dorks interactively operator by operator, batch-run dork lists from file, and export results to TXT / JSON reports.

---

## 📌 Overview

OIndex wraps Google dorking into a full interactive interface — covering login panels, exposed files, config leaks, database errors, sensitive info, cameras, vulnerability candidates, and cloud storage exposure. Supports browser-open, auto-search via `googlesearch-python`, and URL-list export to `oindex_reports/`.

> ⚠️ **Authorised OSINT and security research only.**

---

## 🖥️ Modules

| # | Module | Description |
|---|--------|-------------|
| **[1] Dork Templates** | Browse 50+ ready-made dorks by category — select a template, set a target domain, and open/run/export |
| **[2] Dork Builder** | Build a fully custom dork interactively — add operators, keywords, and exact phrases step by step |
| **[3] Batch Run** | Load a dork list from a `.txt` file and run all dorks in browser-open, auto-search, or URL-list mode |
| **[4] Template Browser** | View and export the full template library to file |

---

## 🗂️ Dork Categories

| # | Category | Count | Coverage |
|---|----------|-------|----------|
| 1 | **login** | 8 | Admin panels, wp-login, cPanel, phpMyAdmin, OWA |
| 2 | **files** | 10 | PDF, Excel, SQL dumps, ENV, config, backup archives |
| 3 | **config** | 10 | web.config, .htaccess, wp-config, Docker, .git, robots.txt |
| 4 | **database** | 6 | SQL errors, DB dumps, MongoDB, phpMyAdmin, Adminer |
| 5 | **info** | 9 | Emails, phone numbers, API keys, AWS creds, private keys, internal IPs |
| 6 | **cameras** | 6 | Webcam interfaces, AXIS cameras, D-Link streams, RTSP, traffic cams |
| 7 | **vulnerabilities** | 8 | Open redirects, LFI/SQLi params, IDOR, admin APIs, directory listing |
| 8 | **cloud** | 8 | S3, Azure Blob, GCP, Firebase, Heroku, Netlify, GitHub secrets |

**Total: 50+ dork templates across 8 categories.**

---

## 🔧 Google Dork Operators (Builder)

| Operator | Description |
|----------|-------------|
| `site:` | Restrict results to a specific domain |
| `inurl:` | Keyword must appear in the URL |
| `intitle:` | Keyword must appear in the page title |
| `intext:` | Keyword must appear in the page body |
| `filetype:` | Restrict to a specific file type |
| `ext:` | Restrict by file extension |
| `cache:` | View Google's cached version of a page |
| `link:` | Pages linking to a specific URL |
| `related:` | Find websites related to a URL |
| `OR` | Boolean OR between terms |
| `-term` | Exclude a specific term |
| `"..."` | Match an exact phrase |
| `*` | Wildcard |

---

## 📥 Input Formats

### Dork Templates
| Input | Description |
|-------|-------------|
| Category | Select one of 8 categories |
| Target Domain | Optional — replaces `{domain}` placeholder in every template |
| Template # | Pick a specific dork from the category list |

### Dork Builder
| Step | Description |
|------|-------------|
| Operator | Add any Google operator with an optional value (e.g. `site:example.com`) |
| Keyword | Add a free-text keyword |
| Exact Phrase | Wrap a phrase in quotes automatically |
| Remove Last | Undo the last added part |

### Batch Run
| Input | Description |
|-------|-------------|
| Dork List File | Plain `.txt` file — one dork per line, `#` for comments |
| Mode | `browser-open`, `auto-search`, or `list-URLs-only` |
| Delay | Configurable seconds between dorks |
| Results per Dork | Number of results to fetch in auto-search mode |

---

## 📤 Output Formats

| Format | Description |
|--------|-------------|
| **Browser Open** | Opens Google search URL directly in your default browser |
| **Auto-Search** | Fetches result URLs via `googlesearch-python` and displays them |
| **URL List** | Builds and saves Google search URLs without executing |
| **TXT Report** | Structured text file with query, domain, category, timestamp, and all result URLs |
| **JSON Report** | Machine-readable output with the same fields plus per-URL entries |

---

## 📁 Reports

All outputs saved to `oindex_reports/`:

| Module | Filename | Key Fields |
|--------|----------|------------|
| Templates / Builder | `oindex_YYYYMMDD_HHMMSS.txt / .json` | query, domain, category, ts, results |
| Batch Run | `oindex_YYYYMMDD_HHMMSS.txt / .json` | dork, url per entry |
| Dork Export | `oindex_dork_YYYYMMDD_HHMMSS.txt` | dork string, Google URL |
| Template Export | `oindex_templates_YYYYMMDD_HHMMSS.txt` | full template library |

---

## ⚙️ Requirements

- **Linux or Windows**
- **No external dependencies for core usage** — stdlib only
- **Optional:** `pip install googlesearch-python` — enables auto-search mode

```bash
# Optional — for auto-search
pip install googlesearch-python
```

Without `googlesearch-python`, browser-open and URL-list modes work fully.

---

## 🚀 Usage

```bash
./OIndex
```

---

## 📄 Batch File Format

```
# My dork list — one dork per line
site:example.com filetype:pdf
site:example.com inurl:admin login
site:example.com intext:"api_key"
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*

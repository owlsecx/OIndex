# 🦉 OIndex

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OReconnaissance-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-2.0-cyan?style=flat-square"/>
</p>

> **OIndex** — Google Dork Builder & OSINT Search

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OIndex builds, organises, and runs Google-dork style OSINT queries from a large template library. Operators can target a domain, pick categories, supply custom or batch dorks, and either auto-search or print URLs offline. HTML-oriented reporting supports authorised open-source collection.

---

## ✨ Features

- 100+ built-in dork templates across many categories
- Domain substitution into templates via -d/--domain
- Category runs, custom -q queries, and batch dork files
- Multi-engine backend selection with result count and delay controls
- Offline --print-urls mode with no browser or network
- List-categories helper for template discovery

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OIndex -d example.com -c files --print-urls
./OIndex -d example.com -c exposed --num 10 --delay 2
./OIndex -q 'site:example.com ext:log' --print-urls
./OIndex --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*

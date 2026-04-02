# ⚒️ OForge

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OPassword%20%2F%20Wordlist%20Generation-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OForge** is a fast and flexible mask-based wordlist generator. Supports standard charsets, custom slots (?1–?4), rule engine (leet, case transformations, append/prepend, years, numbers), stats preview, batch generation from file, progress bar, and automatic TXT export.

---

## 📌 Overview

OForge allows security professionals and researchers to generate highly targeted wordlists using mask patterns similar to Hashcat. It includes a powerful rule engine for post-generation transformations, real-time progress tracking, combination estimation, and support for both single-mask and batch processing. All operations use only the Python standard library.

---

## 🖥️ Modules

| # | Module              | Description |
|---|---------------------|-------------|
| **[1]** | **Generate**            | Single mask → wordlist with optional rules and limit |
| **[2]** | **Batch**               | Process multiple masks from a text file (combined output) |
| **[3]** | **Custom Charsets**     | Define and manage custom character sets (?1 ?2 ?3 ?4) |
| **[4]** | **Rule Preview**        | Test rules on a base word and preview/export variants |

---

## 📊 Key Features

### Charset Tokens
- `?l` → lowercase a-z
- `?u` → uppercase A-Z
- `?d` → digits 0-9
- `?s` → special characters
- `?h` / `?H` → hex (lower/upper)
- `?a` → all printable characters
- `?1`–`?4` → user-defined custom slots

### Rule Engine
Supports the following transformations:
- `upper` / `lower` / `capitalize`
- `reverse`
- `leet` (a→4, e→3, i→1, o→0, s→5, t→7)
- `append:TEXT` / `prepend:TEXT`
- `append_year` (1990–2026)
- `append_num` (00–99)
- `toggle` (swap case per character)

### Statistics & Preview
- Live combination count and estimated file size
- Estimated generation time
- Real-time progress bar with words-per-second
- Warning for very large masks (> 1 billion combinations)

---

## 📁 Output

All generated wordlists are saved to the `oforge_output/` directory:

- Single generation: `oforge_YYYYMMDD_HHMMSS.txt`
- Batch generation: `oforge_batch_YYYYMMDD_HHMMSS.txt`
- Rule preview export: `oforge_rules_YYYYMMDD_HHMMSS.txt`

---

## ⚙️ Requirements

- **Linux or Windows**
- **No Python installation needed** — runs as a standalone executable
- **No external dependencies** — stdlib only

---

## 🚀 Usage

```bash
./OForge

📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED SECURITY TESTING USE ONLY

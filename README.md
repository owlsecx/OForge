# 🦉 OForge

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OPass-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OForge** — Mask Wordlist & Policy Checker

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OForge generates targeted wordlists from mask patterns and checks them against password-policy style constraints. Custom charsets, rule application, batch masks, deduplication, and stats preview help password auditors build coverage sets for authorised cracking labs and policy validation—not indiscriminate attacks.

---

## ✨ Features

- Mask-based wordlist generation with custom ?1–?4 charsets
- Batch masks from a file and optional rule application
- Mask analyse mode to preview stats before generation
- Deduplication modes and output limits for large sets
- Policy-oriented checking alongside generation
- Buffered TXT export under a dedicated output directory

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OForge --mask '?u?l?l?l?d?d?d?d' --limit 10000
./OForge --analyse '?l?l?l?d?d'
./OForge --batch masks.txt --dedup --output oforge_output/words.txt
./OForge --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*

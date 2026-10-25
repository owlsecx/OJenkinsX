# 🦉 OJenkinsX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OJenkinsX** — Offline Jenkins Controller Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OJenkinsX — Offline Jenkins Controller Auditor. It provides offline JENKINS_HOME auditor — no network, no API, strictly read-only, never decrypts any secret; Hardened XML loader — refuses DOCTYPE / ENTITY, size-capped, XML 1.1 declaration tolerant. Built-in demo/self-test paths and severity gates help validate detections without touching production when those flags are used.

---

## ✨ Features

- Offline JENKINS_HOME auditor — no network, no API, strictly read-only, never decrypts any secret
- Hardened XML loader — refuses DOCTYPE / ENTITY, size-capped, XML 1.1 declaration tolerant
- Global config.xml checks — useSecurity, realm, authorization strategy, anonymous read, matrix grants, CSRF crumb issuer, agent protocols, agent port, remember-me, raw-HTML markup, controller executors, signup, agent→cont
- Location config (http:// URL), CLI, API token policy, initialAdminPassword leftovers
- credentials.xml plaintext vs encrypted secrets, secrets/ + master.key + hudson.util.Secret perms
- users/*/config.xml — legacy API tokens, admin count, non-bcrypt password hashes

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OJenkinsX                                     # interactive menu
./OJenkinsX --home /var/lib/jenkins --scan
./OJenkinsX --demo
./OJenkinsX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*

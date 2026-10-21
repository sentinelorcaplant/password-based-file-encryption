# 🏥 Password-Based File Encryption — Complete Guide

<div align="center">

![File Encryption](https://img.shields.io/badge/File-Encryption-0F766E?style=for-the-badge&logo=letsencrypt&logoColor=white)
![AES-256](https://img.shields.io/badge/AES--256-GCM-7C3AED?style=for-the-badge&logo=gnuprivacyguard&logoColor=white)
![Zero Knowledge](https://img.shields.io/badge/Zero-Knowledge-EC4899?style=for-the-badge&logo=1password&logoColor=white)
![Downloads](https://img.shields.io/badge/Downloads-96K-EA580C?style=for-the-badge&logo=download&logoColor=white)

### 🔐 Encrypt Any File with a Password — Strong, Simple, Portable

*A complete guide to password-based file encryption for personal and professional use*

</div>

<img width="1667" height="943" alt="466286f8-a01e-40f3-8bda-cc385774a2c5" src="https://github.com/user-attachments/assets/bff0f5c2-3968-4212-8c96-7e6d48493ef6" />


---

## 🧭 Start by Scenario

> **🎯 What are you encrypting?**

<table>
<tr>
<td width="20%" align="center">

### 📄 Personal

**Documents & photos**

**[Overview](#-overview)**
**[Quick Start](#-quick-start)**
**[Best Practices](#-best-practices)**

</td>
<td width="20%" align="center">

### 💼 Business

**Client files**

**[Compliance](#-compliance-notes)**
**[Key Management](#-key-management)**
**[Sharing Safely](#-safe-sharing-workflow)**

</td>
<td width="20%" align="center">

### 👨‍💻 Developer

**Automate encryption**

**[CLI Reference](#-cli-reference)**
**[API](#-api-reference)**
**[Integration](#-integration-examples)**

</td>
<td width="20%" align="center">

### 🛡️ Security

**Understand the crypto**

**[Algorithm](#-algorithm-details)**
**[Threat Model](#-threat-model)**
**[Auditing](#-security-auditing)**

</td>
<td width="20%" align="center">

### 🛟 Fix

**Troubleshooting**

**[Lost Password](#-lost-password-scenarios)**
**[FAQ](#-faq)**
**[Troubleshooting](#-troubleshooting)**

</td>
</tr>
</table>

---

## 🎯 Overview

**Password-Based File Encryption** is a modern, cross-platform tool that encrypts any file using a **single password** — no accounts, no key servers, no cloud dependency. It uses **AES-256-GCM** with **Argon2id** key derivation, producing an encrypted container that only the correct password can open.

The design philosophy is radical simplicity: **one password, one file, complete control.** Nothing leaves your device. Nothing depends on a service. The encrypted file is a self-contained blob you can store anywhere — USB, cloud, email — without trusting any of them.

### 🧩 What It Does

| Capability | Details |
|-----------|---------|
| 🔐 **Encrypt any file** | Any type, any size |
| 🔑 **Password-protected** | Only your password decrypts |
| 🧂 **Argon2id KDF** | Resists brute force |
| 🛡️ **AES-256-GCM** | Authenticated encryption |
| 📦 **Single output file** | Portable `.enc` container |
| 🌍 **Cross-platform** | Windows, macOS, Linux |
| 📴 **Fully offline** | No network needed |
| 🔌 **CLI + GUI + API** | Any workflow |

---

## 🧬 Core Concepts

| Term | Meaning |
|------|---------|
| 🔐 **Ciphertext** | Encrypted bytes |
| 🔑 **Password** | Your secret |
| 🧂 **Salt** | Random per-file |
| 🧠 **KDF** | Password → key (Argon2id) |
| 🛡️ **AEAD** | Authenticated encryption (GCM) |
| 📦 **Container** | `.enc` file with metadata |
| 🔄 **Nonce** | Unique per encryption |
| 🧾 **Auth tag** | Tamper detection |

---

## 🖥️ System Requirements

### 🔹 Minimum

```
✅ OS: Windows 10, macOS 11+, Ubuntu 20.04+
✅ CPU: Dual-core 2.0 GHz
✅ RAM: 2 GB (4 GB for Argon2 high memory mode)
✅ Storage: 100 MB + space for output files
✅ Runtime: Node.js 18+ or Python 3.10+
✅ No network required
```

### 🔸 Recommended

```
⭐ OS: Windows 11 / macOS 13+ / Ubuntu 22.04+
⭐ CPU: Quad-core 2.5 GHz+
⭐ RAM: 8 GB
⭐ Storage: SSD for larger files
⭐ Runtime: Python 3.11+ / Node.js 20 LTS
⭐ Backup: External drive for encrypted copies
⭐ Password manager: Bitwarden, 1Password, KeePassXC
```

<div align="center">

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-0F766E?style=for-the-badge&logo=letsencrypt&logoColor=white&labelColor=134E4A)](https://share.google/lyrthMPQFuSLZkWxE)

</div>

---

## 📘 Get Instructions

<div align="center">

### 🚀 Access the Official Setup Guide

Click below to reach the instructions portal:

<br>

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-7C3AED?style=for-the-badge&logo=letsencrypt&logoColor=white&labelColor=4C1D95)](https://share.google/lyrthMPQFuSLZkWxE)

<br>

*Open Source • Audited • Updated 2025*

</div>

### 📚 Available Guides

| Guide | Purpose |
|-------|---------|
| 📘 **Getting Started** | Encrypt your first file |
| 📗 **Security Guide** | Algorithm and threat model |
| 📙 **CLI Guide** | Automate encryption |
| 📕 **Sharing Guide** | Send encrypted files safely |
| 📓 **Recovery Guide** | What to do if you forget |

---

## 🚀 Quick Start

### 🪜 Step 1 — Access the Instructions

Open the official setup guide from the button above.

### 🪜 Step 2 — Install

```bash
pip install filecrypt
```

Or with npm:

```bash
npm install -g filecrypt
```

### 🪜 Step 3 — Encrypt a File

```bash
filecrypt encrypt secret.pdf
```

You'll be prompted for a password twice.

### 🪜 Step 4 — Verify Output

```
secret.pdf → secret.pdf.enc
```

<div align="center">

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-16A34A?style=for-the-badge&logo=letsencrypt&logoColor=white&labelColor=14532D)](https://share.google/lyrthMPQFuSLZkWxE)

</div>

### 🪜 Step 5 — Decrypt

```bash
filecrypt decrypt secret.pdf.enc
```

The original file is restored.

### 🪜 Step 6 — Test with the Wrong Password

Try decrypting with an incorrect password — the file will be **rejected**, not corrupted.

### 🪜 Step 7 — Store Safely

Move `.enc` files to backups, cloud, USB — anywhere.

### 🪜 Step 8 — Delete the Original

Once encrypted and verified, securely delete the plaintext.

---

## 🔐 Algorithm Details

### 🧠 Encryption Stack

| Layer | Algorithm | Purpose |
|-------|-----------|---------|
| 🧂 **KDF** | Argon2id | Slow brute force |
| 🔐 **Cipher** | AES-256-GCM | Encrypt + authenticate |
| 🎲 **Nonce** | 96-bit random | Unique per file |
| 📦 **Format** | Custom container | Self-describing |
| 🧾 **Integrity** | GCM tag | Detect tampering |

### 🧪 Argon2id Parameters

| Parameter | Default | Notes |
|-----------|:-------:|-------|
| Memory | 64 MB | Higher = stronger |
| Iterations | 3 | More = slower |
| Parallelism | 4 | Cores used |
| Salt | 16 bytes | Random per file |

> **💡 Why Argon2id?** It's the current standard for password hashing — memory-hard, GPU-resistant, and winner of the Password Hashing Competition.

### 🔒 Container Format

```
┌──────────────────────────────────────┐
│ Magic bytes  "FCRY"          (4B)    │
│ Version                       (1B)    │
│ KDF params                    (16B)   │
│ Salt                          (16B)   │
│ Nonce                         (12B)   │
│ Ciphertext + auth tag    (variable)   │
└──────────────────────────────────────┘
```

---

## 🛡️ Threat Model

### ✅ What This Protects Against

| Threat | Protection |
|--------|------------|
| 🕵️ **Stolen drive** | Strong encryption |
| ☁️ **Compromised cloud** | Zero-knowledge |
| 📧 **Intercepted email** | Authenticated cipher |
| 🗂️ **File tampering** | GCM tag detects it |
| 🧪 **Brute force** | Argon2id slows attacks |

### ❌ What It Doesn't Protect Against

| Threat | Why |
|--------|-----|
| 🎥 **Malware on your PC** | Can capture passwords |
| 🔑 **Weak passwords** | Always the weakest link |
| 🧑 **Someone watching you type** | Physical security |
| 💀 **Forgotten password** | No recovery — by design |
| 🎯 **Coerced disclosure** | You can be forced to reveal |

---

## 🔑 Key Management

### 🧠 Best Practices

| Practice | Why |
|----------|-----|
| 🎲 **Strong password** | 4+ random words |
| 💾 **Store in manager** | Bitwarden, KeePassXC |
| 🔁 **Unique per file** | Limits blast radius |
| 📝 **Backup password** | Securely, offline |
| 🚫 **Don't email password** | Use a separate channel |
| 🔄 **Rotate for sensitive** | Defense over time |

### 🎲 Strong Password Examples

| Password | Strength |
|----------|:--------:|
| `correct-horse-battery-staple` | ✅ Strong |
| `Tr0ub4dor&3` | ⚠️ Weak |
| `xK9$mQ2!LwPz` | ✅ Strong but hard |
| `crimson-violin-echo-harbor` | ✅ Best |

> **💡 Rule:** 4+ random words = strong *and* memorable.

---

## 🤝 Safe Sharing Workflow

### 🪜 Step 1 — Encrypt the File

```bash
filecrypt encrypt contract.pdf --password
```

### 🪜 Step 2 — Send the File Separately

Email, cloud, or USB.

### 🪜 Step 3 — Send the Password via a Different Channel

SMS, voice call, or in person — **never the same channel**.

### 🪜 Step 4 — Recipient Decrypts

```bash
filecrypt decrypt contract.pdf.enc
```

### 🪜 Step 5 — Confirm Receipt

Recipient confirms decryption succeeded.

### 🪜 Step 6 — Delete Securely

Both parties securely delete the file if needed.

---

## 💻 CLI Reference

| Command | Purpose |
|---------|---------|
| `filecrypt encrypt <file>` | Encrypt a file |
| `filecrypt decrypt <file>` | Decrypt a file |
| `filecrypt encrypt --password` | Prompt for password |
| `filecrypt encrypt --out <path>` | Custom output |
| `filecrypt batch <glob>` | Encrypt many |
| `filecrypt verify <file>` | Check integrity |
| `filecrypt shred <file>` | Secure delete |
| `filecrypt --version` | Show version |

### 🧪 Examples

```bash
# Encrypt with a password
filecrypt encrypt notes.txt --password

# Decrypt into a specific folder
filecrypt decrypt notes.txt.enc --out ./restored/

# Batch encrypt a folder
filecrypt batch ./documents/*.pdf --password

# Verify integrity of an encrypted file
filecrypt verify notes.txt.enc
```

---

## 🔌 API Reference

### 📦 Node.js

```javascript
const { encrypt, decrypt } = require('filecrypt');

const encrypted = await encrypt({
  input: 'secret.pdf',
  password: 'my strong password',
  output: 'secret.pdf.enc'
});

const decrypted = await decrypt({
  input: 'secret.pdf.enc',
  password: 'my strong password',
  output: 'secret.pdf'
});
```

### 🐍 Python

```python
from filecrypt import encrypt_file, decrypt_file

encrypt_file('secret.pdf', 'secret.pdf.enc', 'my strong password')
decrypt_file('secret.pdf.enc', 'secret.pdf', 'my strong password')
```

---

## ⚙️ Integration Examples

### 🔄 Backup Pipeline

```bash
#!/bin/bash
for f in ~/Documents/*; do
  filecrypt encrypt "$f" --password
done
```

### 🔐 Encrypted Upload

```bash
filecrypt encrypt local.zip
scp local.zip.enc user@backup.example.com:/backups/
```

### 🧾 Signed + Encrypted

```bash
gpg --sign document.pdf
filecrypt encrypt document.pdf.gpg --password
```

---

## 🏛️ Compliance Notes

| Standard | Relevance |
|----------|-----------|
| 📜 **GDPR** | Encrypting personal data |
| 🏥 **HIPAA** | Medical records |
| 💳 **PCI-DSS** | Cardholder data |
| 🔐 **ISO 27001** | Info security |
| 📊 **SOC 2** | Controls |
| ⚖️ **ITAR/EAR** | Export-controlled |

> **📌 Note:** Encryption alone isn't compliance. Document your policies, manage keys, and train users.

---

## 🧪 Security Auditing

### 🔍 Verify Your Copy

```bash
sha256sum filecrypt.enc
```

### 🧪 Test Decryption

Use a test file first — always verify before deleting originals.

### 🕵️ Check Container Integrity

```bash
filecrypt verify secret.pdf.enc
```

Output:

```
✓ Valid container
✓ Authentication tag matches
✓ No tampering detected
```

---

## 🚑 Lost Password Scenarios

### ⚠️ The Hard Truth

> **🛑 If you lose your password, the file is gone.**
>
> This is by design. There is no recovery, no backdoor, no admin reset. Encryption is only as strong as the fact that **you cannot bypass it**.

### 🛡️ Prevention Checklist

- ✅ Store passwords in a manager
- ✅ Create an encrypted backup of the password file
- ✅ Write down a recovery copy and store offline
- ✅ Use a password hint stored separately
- ✅ Test decryption before deleting originals

---

## 🧪 Verification

| Check | Command | Expected |
|-------|---------|----------|
| ✅ Install | `filecrypt --version` | Version shown |
| ✅ Encrypt works | `encrypt` | `.enc` created |
| ✅ Decrypt works | `decrypt` | File restored |
| ✅ Wrong password | Attempt | Fails cleanly |
| ✅ Tamper detection | Modify byte | Verify fails |
| ✅ Batch works | `batch` | All encrypted |
| ✅ Verify works | `verify` | Passes |
| ✅ Shred works | `shred` | File gone |

---

## 🩺 Troubleshooting

| Problem | Cause | Solution |
|---------|-------|----------|
| 🚫 Can't decrypt | Wrong password | Retry with correct |
| 🚫 File corrupted | Interrupted write | Use backup |
| 🚫 Slow encryption | High Argon2 mem | Lower parameter |
| 🚫 Out of memory | Large file | Increase RAM |
| 🚫 API error | Wrong parameter | Check docs |
| 🚫 File not found | Wrong path | Verify path |
| 🚫 Permission denied | Filesystem | Run as user |
| 🚫 Cross-platform issue | Version mismatch | Match versions |
| 🚫 Container invalid | Not `.enc` | Check format |
| 🚫 Slow on SSD | I/O bound | Use NVMe |

### 🔄 Reset Config

```bash
filecrypt config --reset
```

---

## 📚 Resources

| Resource | Purpose |
|----------|---------|
| 📖 **Official Docs** | Full reference |
| 🔐 **Cryptography Guide** | Learn the theory |
| 💬 **Community** | Help |
| 🎥 **Video Guides** | Walkthroughs |
| 📊 **Benchmarks** | Performance |

---

## 💬 FAQ

**Is this safe to use?**
Yes — with strong passwords and trusted binaries.

**Do you store my password?**
Never — it stays on your device.

**What if I forget my password?**
The file is unrecoverable — this is the point.

**Which algorithm is used?**
AES-256-GCM with Argon2id.

**Can I encrypt multiple files?**
Yes — via batch mode.

**Does it work offline?**
Yes — fully offline.

**Is it open source?**
Yes — MIT license.

**Can I use it in production?**
Yes — after auditing the source.

**Does it work on mobile?**
Yes — web version available.

**How large can files be?**
Up to the size of your storage.

---

## 📅 Version History

| Version | Date | Highlights |
|---------|------|-----------|
| **2.3.0** | Jan 2025 | Argon2id default |
| 2.1.0 | Oct 2024 | Batch mode |
| 2.0.0 | Jun 2024 | New container format |
| 1.5.0 | Feb 2024 | Initial release |

---

<div align="center">

### 🌟 Found This Guide Helpful?

[![Get Instructions](https://img.shields.io/badge/📘_GET_INSTRUCTIONS-EA580C?style=for-the-badge&logo=letsencrypt&logoColor=white&labelColor=7C2D12)](https://share.google/lyrthMPQFuSLZkWxE)

**⭐ Star this repository if it helped! ⭐**

*Made with 💜 for the security community*

</div>

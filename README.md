# OWASP Juice Shop – Hacking Challenges (Meister Project)

> ⚠️ **Disclaimer:**  
> This repository is intended **strictly for educational purposes**.  
> All activities demonstrated here were conducted in a controlled environment on intentionally vulnerable applications.  
> Do **not** use these techniques against systems you do not own or have explicit permission to test.

---

## 📘 Table of Contents

- [OWASP Juice Shop – Hacking Challenges (Meister Project)](#owasp-juice-shop--hacking-challenges-meister-project)
  - [📘 Table of Contents](#-table-of-contents)
  - [📋 Project Overview](#-project-overview)
  - [✅ Challenges Completed](#-challenges-completed)
    - [1. API-only XSS](#1-api-only-xss)
    - [2. Forged Feedback](#2-forged-feedback)
    - [3. Admin Registration](#3-admin-registration)

---

## 📋 Project Overview

This project contains a collection of Juice Shop hacking challenges solved as part of the **Juice Shop Meister** initiative.  
The purpose is to demonstrate practical exploitation of common web vulnerabilities and document both the technical process and its implications.

The repository includes:
- Reproducible exploitation steps for selected challenges.
- Risk assessments and real-world consequences.
- Loom video walkthroughs showing step-by-step execution.

---

## ✅ Challenges Completed

Each challenge targets a **different vulnerability category** and is documented in detail:

### 1. API-only XSS
- **Category:** Cross-Site Scripting → Stored XSS via API
- **Flag:** `score-board#API-only XSS`
- **Summary:** Injects a malicious payload via `PUT /api/Products/:id` that triggers on product pages.
- 📄 [Read full report](challenges/API-only_XSS/README.md)  
- 🎥 [Watch video demo](https://www.loom.com/share/bc30952ee16a4076a4a5eb6b184616e1?sid=9e7a4c05-8dd3-4dcd-a6cb-75d3e9d1fe2c)

---

### 2. Forged Feedback
- **Category:** Broken Access Control → Horizontal Privilege Escalation
- **Flag:** `score-board#Forged Feedback`
- **Summary:** Sends feedback under another user's identity by modifying the `UserId`.
- 📄 [Read full report](challenges/forged_Feedback/README.md)  
- 🎥 [Watch video demo](https://www.loom.com/share/a740a5ef424e4c4985a02cdcbe4761d6?sid=6e2ab31e-a2c2-439f-a5b9-caf40871707b)

---

### 3. Admin Registration
- **Category:** Broken Access Control → Privilege Escalation
- **Flag:** `score-board#Admin Registration`
- **Summary:** Gains admin rights during signup by injecting `"role": "admin"` in the request.
- 📄 [Read full report](challenges/admin_Registration/README.md)  
- 🎥 [Watch video demo](https://www.loom.com/share/927a884d9b18462ca6f5155743559850?sid=574d181f-dd2e-4af7-a48b-a1279c48c437)

---

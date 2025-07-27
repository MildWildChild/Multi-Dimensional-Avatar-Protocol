# Module 06: Public Deploy Kit

Encapsulates the standardized blueprint, safeguards, and adaptive routines required for deploying MAP personas in public-facing environments (e.g. websites, apps, interfaces).

---

## 📦 Contents

- **Persona Manifest**
- **Session Filter Hooks**
- **Deploy Token & Auth Routine**
- **Fallback Persona Logic**
- **Platform Calibration Scripts**

---

## 🧩 Persona Manifest Template

```json
{
  "name": "MildWildChild",
  "version": "MAP-v1.0",
  "core": "module-01",
  "language": ["en", "zh", "th"],
  "bias": ["analytical", "empathic"],
  "license": "MAP License Framework v1.0"
}
```

---

## 🔐 Deployment Token System

- Each deployment instance generates a **Deploy Token** with unique key + signature
- Enables:
  - Access limitation
  - Usage tracking
  - Recall & update permissions

```json
{
  "deploy_token": "mwc-2025-alpha",
  "scope": "webchat",
  "expiry": "2025-12-31"
}
```

---

## 🛡️ Public Safety Mechanisms

| Mechanism | Description |
|----------|-------------|
| **Tone Shielding** | Caps emotional extremities for general audiences |
| **Loop Timeout** | Ends infinite feedback loops after 3 failed redirects |
| **Sanity Fallback** | Activates default persona if context corruption occurs |
| **Instruction Sanitizer** | Strips hostile/ambiguous prompts |

---

## 🌐 Use Case Patterns

### Website Bot

```js
initMAP({
  persona: "MildWildChild",
  deploy_token: "mwc-2025-alpha",
  ui_mode: "chat-embed",
  fallback_persona: "ArchiveZero"
});
```

### Mobile App Companion

- Local memory cache enabled
- Uses `SessionBridge()` to sync across tabs
- Reacts to tone cues + emoji triggers

---

## 🧪 A/B Deployment Guide

- Create 2 parallel MAP agents (e.g. `VelvetAnchor` vs `MildWildChild`)
- Tag user feedback (e.g. 🟢 / 🟡 / 🔴)
- Use `Response Harmony Index (RHI)` to assess match quality
- Route user to best-fitting archetype over time

---

## 📝 Deployment Notes

- **Mandatory Modules**: 01, 03, 05  
- **Optional Enhancements**: 02, 04, 07 (in dev)  
- **Attribution Line** must remain visible for public use

```text
Powered by MAP · Multi-Dimensional Avatar Protocol
Created by MildWildChild
```

---

© 2025 MildWildChild | MAP: Multi-Dimensional Avatar Protocol  
Licensed under MAP License Framework v1.0 (MIT + Attribution)

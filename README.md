<p align="center">
  <img src="https://img.shields.io/badge/AWS-CloudTrail-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/v2.0-00C853?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Zero_Dependencies-7B1FA2?style=for-the-badge" />
  <img src="https://img.shields.io/badge/100%25_Client--Side-0288D1?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" />
</p>

<h1 align="center">☁️ CloudTrail Viewer</h1>

<p align="center">
  <strong>A lightweight, single-file web app to inspect AWS CloudTrail logs instantly.</strong><br>
  Drop a CloudTrail JSON file → see what matters. No server, no dependencies, no data leaving your machine.
</p>

---

## ✨ Features

| Feature | Description |
|---|---|
| 📂 **Drag & Drop Upload** | Drop one or multiple `.json` CloudTrail files — parsed instantly |
| 📊 **Insights Dashboard** | Expandable cards showing unique value counts for Event Name, Source IP, User Agent, User/Role, Read Only, Category & Error Code |
| ☑️ **Dashboard Filters** | Expand any dashboard card to see all unique values with checkboxes — select specific values to filter the table |
| 📈 **Summary Stats Bar** | Total events, unique event names, unique IPs, and time range at a glance |
| 🔃 **Sortable Columns** | Click any header to sort ascending/descending |
| 🔍 **Global Search** | Free-text search across all fields in real-time |
| ⧩ **Per-Column Filters** | Click the filter icon on any column header to filter by specific values |
| ⚙️ **Column Toggles** | Show/hide any of the 17 extracted columns to focus on what matters |
| 📋 **Detail Modal** | Click any row to see the full raw JSON with syntax highlighting |
| 🏷️ **Color-Coded Badges** | Root (amber), IAMUser (purple), AssumedRole (cyan), Read (green), Write (red) |
| 🎨 **Dark Glassmorphism UI** | Modern dark theme with smooth animations and micro-interactions |

## 🆕 What's New in v2.0

- **📊 Insights Dashboard** — expandable summary cards between stats bar and search toolbar
- **☑️ Selectable unique values** — each card expands to show all unique values with counts, mini bar charts, and checkboxes
- **🔗 Full-width expand** — expanded cards span the full page width with smooth animation, showing complete values (no truncation)
- **⚙️ Redesigned Columns button** — premium gradient style with glow effect
- **☁️ New cloud logo** — custom SVG cloud icon with trail lines

## 🚀 Quick Start

1. **Clone the repo**
   ```bash
   git clone https://abdurrahman-cybersec/cloudtrail-viewer.git
   ```

2. **Open the file**
   ```bash
   # Just open in your browser — that's it!
   open cloudtrail-viewer.html        # macOS
   xdg-open cloudtrail-viewer.html    # Linux
   start cloudtrail-viewer.html       # Windows
   ```

3. **Drop a CloudTrail JSON file** onto the upload area

> No `npm install`, no build step, no server. It's a single HTML file.

## 📸 What You'll See

After dropping a CloudTrail JSON file:

- **Stats bar** — event count, unique events, unique IPs, time range
- **Insights Dashboard** — 7 expandable cards showing unique value breakdowns with selectable checkboxes
- **Filterable table** — sort by any column, filter by specific values
- **Color-coded badges** — identity types and read/write status
- **Click any row** — full JSON detail modal with syntax highlighting

## 🔐 Privacy & Security

- **100% client-side** — your CloudTrail data never leaves your browser
- **No external requests** — no analytics, no tracking, no APIs
- **No dependencies** — just vanilla HTML, CSS, and JavaScript

## 📁 Supported Format

Standard AWS CloudTrail JSON files:
```json
{
  "Records": [
    {
      "eventVersion": "1.08",
      "eventTime": "2023-08-26T20:54:28Z",
      "eventName": "AssumeRole",
      "eventSource": "sts.amazonaws.com",
      "sourceIPAddress": "84.32.71.33",
      "userAgent": "aws-cli/1.27.74 ...",
      ...
    }
  ]
}
```

## 🛡️ Use Cases

- **Incident Response** — quickly triage CloudTrail events during an investigation
- **Security Auditing** — filter by source IP, user agent, or identity type to spot anomalies
- **CTF / Cloud Forensics** — parse challenge CloudTrail files without uploading to third-party tools
- **Learning AWS** — understand what API calls your account is making

## 📝 License

MIT — use it, fork it, share it.

---

<p align="center">
  <strong>⭐ Star this repo if you find it useful!</strong>
</p>

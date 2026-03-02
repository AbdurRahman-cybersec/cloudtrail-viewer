<p align="center">
  <img src="https://img.shields.io/badge/AWS-CloudTrail-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Zero_Dependencies-00C853?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Runs_Locally-7B1FA2?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" />
</p>

<h1 align="center">☁️ CloudTrail Viewer</h1>

<p align="center">
  <strong>A lightweight, single-file web app to inspect AWS CloudTrail logs instantly.</strong><br>
  Drop a CloudTrail JSON file → see what matters. No server, no dependencies, no data leaving your machine.
</p>

----
## ✨ Features

| Feature | Description |
|---|---|
| 📂 **Drag & Drop Upload** | Drop one or multiple `.json` CloudTrail files — parsed instantly |
| 📊 **Smart Table View** | 17 key fields extracted, 11 shown by default |
| 🔃 **Sortable Columns** | Click any header to sort ascending/descending |
| 🔍 **Global Search** | Free-text search across all fields in real-time |
| ⧩ **Per-Column Filters** | Click the filter icon on any column to filter by specific values |
| ⚙️ **Column Toggles** | Show/hide any column to focus on what matters |
| 📋 **Detail Modal** | Click a row to see the full raw JSON with syntax highlighting |
| 📈 **Summary Stats** | Total events, unique event names, unique IPs, time range |
| 🎨 **Dark Glassmorphism UI** | Modern dark theme with smooth animations |

![CloudTrail Viewer Screenshot](screenshots/cloudtrail-viewer1.png)
<br>
<br>
<br>
![CloudTrail Viewer Screenshot](screenshots/cloudtrail-viewer2.png)


## 🚀 Quick Start

1. **Clone the repo**
   ```bash
   git clone https://github.com/abdurrahman-cybersec/cloudtrail-viewer.git
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
- **Filterable table** — sort by any column, filter by specific values
- **Color-coded badges** — Root (amber), IAMUser (purple), AssumedRole (cyan), Read (green), Write (red)
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

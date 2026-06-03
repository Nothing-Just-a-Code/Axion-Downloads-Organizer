<p align="center">
  <img src="https://github.com/user-attachments/assets/b4fc0e00-4c73-47ac-8948-671d86ee5432" alt="Axion Downloads Organizer" width="80">
</p>

<h1 align="center">Axion Downloads Organizer</h1>

<p align="center">
  <strong>Automatically organize your Downloads folder in real time.</strong><br>
  A lightweight Windows utility that silently monitors downloads and instantly sorts files into a structured folder hierarchy.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Windows-blue" alt="Platform">
  <img src="https://img.shields.io/badge/license-Personal%20Use-green" alt="License">
  <img src="https://img.shields.io/badge/privacy-100%25%20Local-success" alt="Privacy">
  <img src="https://img.shields.io/badge/telemetry-None-red" alt="Telemetry">
</p>

---

# Overview
<p align="center">
<img width="600" alt="axion logo" src="https://github.com/user-attachments/assets/46322069-f3b6-4b61-a71b-9fcbc908f3e7" />
</p>

**Axion Downloads Organizer** is a smart background utility that automatically keeps your Downloads folder clean and organized without requiring any manual effort.

Once installed, Axion runs quietly in the system tray, starts automatically with Windows, and continuously monitors your Downloads folder. Whenever a download completes or a file is renamed, Axion instantly categorizes and moves it into the appropriate destination folder using a customizable rule engine.

No dragging files. No manual sorting. No clutter.

---

# Features

## Real-Time Organization

Files are organized the moment they become available.

- Continuously monitors your Downloads folder
- Detects completed downloads
- Detects renamed files
- Automatically creates missing folders
- Runs silently in the background

## Intelligent Categorization

Automatically sorts files into logical categories based on type.

- Images
- Audio
- Videos
- Documents
- Source Code
- Archives
- Applications
- Databases
- Fonts
- 3D Models
- And many more

## Smart Image Detection

Axion goes beyond simple file extensions.

Small PNG and ICO files are automatically detected as application icons based on their dimensions.

| Type | Detection |
|--------|-----------|
| App Icons | PNG/ICO ≤ 256×256 pixels |
| Wallpapers | Larger image files |
| GIFs | Animated image formats |
| Raw Images | Camera RAW formats |
| Screenshots | Rule-based classification |

Image dimension analysis runs before normal rules are evaluated, ensuring accurate placement.

## Fully Customizable Rules

Every rule can be customized through a simple JSON configuration file.

You can:

- Add new rules
- Disable existing rules
- Reorder rules
- Change destination folders
- Create custom categories
- Extend supported file types

Rules are processed from top to bottom and the first match wins.

## Safe File Handling

Axion is designed to prevent data loss.

- Ignores incomplete downloads
- Ignores temporary browser files
- Avoids moving files still being written
- Handles duplicate filenames safely
- Multiple conflict resolution modes

## System Tray Integration

- Runs quietly in the notification area
- Starts automatically with Windows
- Minimal CPU usage
- Minimal memory consumption

---

# How It Works

1. A file is downloaded or renamed.
2. Axion detects the change.
3. Temporary download files are ignored.
4. File extension is analyzed.
5. Supported image files may be inspected for dimensions.
6. Rules are evaluated from top to bottom.
7. The first matching rule determines the destination.
8. The file is moved automatically.

Folders are created automatically when required.

---

# Default Folder Structure

```text
Downloads
├─ Pictures
│  ├─ Wallpapers
│  ├─ App Icons
│  ├─ GIFs
│  ├─ Vector
│  ├─ Raw
│  └─ Screenshots
│
├─ Audio
│  ├─ Music
│  └─ Wav
│
├─ Videos
│
├─ Documents
│  ├─ eBooks
│  ├─ Fonts
│  └─ 3D Models
│
├─ MS Office
│  ├─ Spreadsheets
│  └─ Presentations
│
├─ Codes
│  ├─ VB.NET
│  ├─ C#
│  ├─ Python
│  ├─ JavaScript
│  ├─ Web
│  ├─ Java
│  ├─ C++
│  ├─ PHP
│  ├─ Ruby
│  ├─ Go
│  ├─ Rust
│  ├─ Swift
│  └─ Config
│
├─ Applications
│  └─ Disk Images
│
├─ Archives
│
└─ MySQL
```

Axion ships with support for hundreds of common file extensions.

---

# Supported Categories

## Images

```text
PNG
JPG
JPEG
WEBP
BMP
ICO
GIF
SVG
RAW
PSD
AI
```

## Audio

```text
MP3
WAV
FLAC
AAC
M4A
OGG
```

## Video

```text
MP4
MKV
AVI
MOV
WEBM
WMV
```

## Documents

```text
PDF
TXT
RTF
EPUB
MOBI
DOCX
```

## Archives

```text
ZIP
RAR
7Z
TAR
GZ
BZ2
```

## Programming Languages

```text
VB.NET
C#
Python
JavaScript
TypeScript
Java
C++
PHP
Ruby
Go
Rust
Swift
HTML
CSS
JSON
XML
YAML
```

## Databases

```text
SQL
DB
SQLITE
MDB
ACCDB
```

---

# Configuration

Axion uses a simple JSON-based rules engine.

Example rule:

```json
{
  "Name": "Python Files",
  "Extensions": [".py"],
  "Destination": "Codes\\Python",
  "Enabled": true
}
```

Rules are evaluated sequentially:

```text
Rule 1
Rule 2
Rule 3
...
```

Once a rule matches, processing stops and the file is moved.

This provides predictable and highly customizable behavior.

---

# File Conflict Handling

When a file already exists in the destination folder, Axion can:

| Mode | Description |
|--------|-------------|
| Rename | Generates a unique filename |
| Overwrite | Replaces the existing file |
| Skip | Leaves the new file untouched |

The behavior can be configured through the settings interface.

---

# Privacy

Axion is designed with privacy as a core principle.

- 100% local operation
- No cloud services
- No user accounts
- No telemetry
- No analytics
- No tracking
- No data collection

Your files never leave your computer.

---

# Performance

Axion is optimized for long-term background operation.

- Lightweight memory usage
- Low CPU consumption
- Fast rule evaluation
- Handles large download bursts
- Reliable file monitoring

Install it once and forget it exists.

---

# Perfect For

### Developers

Keep source code, archives, installers, SDKs, and documentation organized automatically.

### Designers

Separate wallpapers, icons, vectors, fonts, and raw assets without manual sorting.

### Students

Organize PDFs, presentations, spreadsheets, and study materials instantly.

### Office Workers

Maintain a clean Downloads folder and quickly find important documents.

### Power Users

Eliminate clutter and keep a structured file system automatically.

---

# Why Axion?

Most users download dozens of files every day.

Within weeks, the Downloads folder becomes a chaotic mix of installers, documents, images, videos, archives, and temporary files.

Axion solves this problem automatically.

Install it once and enjoy a permanently organized Downloads folder without changing your workflow.

---

# License

**Free for personal and non-commercial use.**

Commercial, educational, government, business, or professional usage requires a separate commercial license.

See the `LICENSE` file for complete licensing information.

---

<p align="center">
  <strong>Axion Downloads Organizer</strong><br>
  Because a clean Downloads folder is the first step toward a productive day.
</p>

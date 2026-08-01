# 🐔 FreeRange Exam Suite (v3.6.0.0)

![Version](https://img.shields.io/badge/version-3.6.0.0-blue.svg)
![Security](https://img.shields.io/badge/security-100%25_Offline_/_Air--Gapped-green.svg)
![Languages](https://img.shields.io/badge/languages-7_Supported-orange.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)
<div align="center">
<img src="Vertical.png" width="900">
</div>

**FreeRange Exam Suite** is a powerful, lightweight, and fully offline desktop suite designed for IT certification exam preparation (Cisco CCNA/CCNP, CompTIA, AWS, Microsoft, etc.). 

The suite consists of two standalone applications:
1. **FreeRange Exam Simulator**: An interactive exam environment featuring realistic exam mechanics, timer controls, detailed topic statistics, and instant answer reviews.
2. **FreeRange Exam Builder**: A visual GUI generator allowing users to create, edit, and export custom exam files in JSON format without writing a single line of code.
<div align="center">
 
| Splash Simulator | Splash Builder |
| :---: | :---: |
| <img src="splash_sim.png" width="400"> | <img src="splash_bui.png" width="400"> |

</div>

---

## ✨ Key Features

### 🚀 Exam Simulator
* **Multiple Question Types**:
  * **Single Choice & Multiple Choice** questions.
  * **Inline Fill-in-the-Blank** (`___` placeholders).
  * **Advanced Drag & Drop**: Full mouse drag-and-drop & click-to-place support for matching, sequencing/ordering (e.g., Step 1 to 5), multi-use answers, and distractors.
* **Exhibit Support**: View attached diagrams and topology images (`.jpg`/`.png` Base64) in high-resolution popups.
* **Topic Filtering**: Selectively study specific topics or domains within an exam.
* **Flexible Modes**: Run full random simulations or test specific question ranges (e.g., Q1 to Q50).
* **Real-time Controls**: Pause/resume timer, shuffle questions/options, and reveal correct answers on the fly.
* **Comprehensive Results**:
  * Visual score vs. passmark comparison bars.
  * Topic-by-topic percentage performance breakdown.
  * Detailed mistake review window.
  * **Export to TXT** and **Copy to Clipboard** features for wrong answers.

### 🛠️ Exam Builder
* **3 Question Creation Modes**: Standard Choice, Fill-in-the-Blank, and Drag & Drop.
* **Visual Drag & Drop Editor**: Easily configure category targets, draggable items, and distractors.
* **Exhibit Image Attachment**: Embed images directly into questions via automatic Base64 encoding.
* **Smart Validation**: Built-in checks prevent broken questions, unmatched blank placeholders, or missing answers.
* **Unsaved Changes Detection**: Prompts alerts to prevent accidental data loss when editing.
* **JSON File Management**: Load, modify, and re-export existing exam files seamlessly.

---

## 🌐 Native Multi-Language Support

Both the Simulator and Builder feature a built-in language selection screen upon launch, supporting **7 languages**:

| Flag | Language | Flag | Language |
| :---: | :--- | :---: | :--- |
| 🇮🇹 | Italian | 🇩🇪 | German |
| 🇬🇧 | English | 🇵🇹 | Portuguese |
| 🇪🇸 | Spanish | 🇨🇿 | Czech |
| 🇫🇷 | French | | |

---

## 🔒 Security & Privacy Architecture

* **100% Offline (Air-Gapped Native)**: Zero outbound network calls (no HTTP/HTTPS or socket connections). No telemetry, no auto-updaters, and no tracking scripts.
* **Local Data Persistence**: Exam files (`.json`) and image exhibits are stored exclusively on local disk storage.
* **GDPR & PII Compliant**: Collects zero personal data or corporate credentials.
* **Standard Privileges**: Operates strictly within the non-privileged user context at runtime.

---

## 🚀 What's New in Version 3.6.0.0

* **Fully Revamped UI**: A completely revised and improved graphical interface, offering a more modern, cleaner, and highly intuitive user experience.
* **Complete Codebase Overhaul**: The underlying application code has been entirely refactored and optimized from the ground up for maximum stability and performance.
* **Evaluation Engine Fix**: Resolved a critical bug where shuffling options caused incorrect grading for Multiple Choice and list-based answers.
* **Dynamic UI Translations**: The "Info/About" screen now fully supports dynamic translations based on the user's selected UI language.
* **Microsoft Store Readiness**: Replaced the legacy installer with a fully compliant MSIX package (`FreeRangeExamSuite_3.6.0.0.msix`), ensuring seamless installation, secure sandboxing, and direct validation through the Microsoft Store.

---

## 📸 Application Screenshots

<div align="center">

### 🚀 Simulator in Action
| Exam Setup | Drag & Drop Mechanics |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(9).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(3).png" width="400"> |

| Fill-in-the-Blank Questions | Exam Results & Analytics |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(4).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(11).jpg" width="400"> |

| Mistakes Report | Single Choice Exhibit |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(10).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(5).png" width="400"> |

| Multiple Choice | Multi-Language Selection |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(7).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(1).png" width="400"> |

<br>

### 🛠️ Exam Builder Engine
| Builder Interface | Question Editor & DND Setup |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(8).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(12).jpg" width="400"> |

| Exhibit Attachment & Preview | Fill-in-the-blank |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(13).jpg" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(14).jpg" width="400"> |

<br>

<details>
<summary><b>🔍 Click here to view all screenshots in full detail (Images 9 & 10)</b></summary>
<br>

<p align="center">
  <img src="screenshots/FreeRange%20Exam%20Suite%20(9).png" width="80%"><br><br>
  <img src="screenshots/FreeRange%20Exam%20Suite%20(10).png" width="80%">
</p>

</details>

</div>

---

## 📦 Installation & Quick Start

### MSIX Package (Recommended)
1. Download `FreeRangeExamSuite_3.6.0.0.exe` from the [Releases](../../releases) section or install it directly via the **Microsoft Store**. (Certification still in progress)
2. Double-click the `.exe` file to launch the native Windows App Installer.
3. Launch **FreeRange Exam Simulator** or **FreeRange Exam Builder** directly from the Start Menu.

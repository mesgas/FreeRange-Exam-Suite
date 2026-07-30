# 🐔 FreeRange Exam Suite (v3.5 - Drag & Drop Edition)

![Version](https://img.shields.io/badge/version-3.5-blue.svg)
![Security](https://img.shields.io/badge/security-100%25_Offline_/_Air--Gapped-green.svg)
![Languages](https://img.shields.io/badge/languages-7_Supported-orange.svg)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)

<img src="Vertical.png" width="900">

**FreeRange Exam Suite** is a powerful, lightweight, and fully offline desktop suite designed for IT certification exam preparation (Cisco CCNA/CCNP, CompTIA, AWS, Microsoft, etc.). 

The suite consists of two standalone applications:
1. **FreeRange Exam Simulator**: An interactive exam environment featuring realistic exam mechanics, timer controls, detailed topic statistics, and instant answer reviews.
2. **FreeRange Exam Builder**: A visual GUI generator allowing users to create, edit, and export custom exam files in JSON format without writing a single line of code.

| Splash Simulator | Splash Builder |
| :---: | :---: |
| <img src="splash_sim.png" width="400"> | <img src="splash_bui.png" width="400"> |

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
| 🇪🇸 | Spanish | 🇳🇱 | Dutch |
| 🇫🇷 | French | | |

---

## 🔒 Security & Privacy Architecture

* **100% Offline (Air-Gapped Native)**: Zero outbound network calls (no HTTP/HTTPS or socket connections). No telemetry, no auto-updaters, and no tracking scripts.
* **Local Data Persistence**: Exam files (`.json`) and image exhibits are stored exclusively on local disk storage.
* **GDPR & PII Compliant**: Collects zero personal data or corporate credentials.
* **Standard Privileges**: Operates strictly within the non-privileged user context at runtime.

---

## 🚀 What's New in Version 3.5

* **True Mouse Drag & Drop**: Native mouse drag interaction for Cisco/CompTIA-style sequencing and matching questions.
* **Unlimited Answer Pool**: Drag-and-drop items remain available in the source list for questions requiring the same answer across multiple targets.
* **Inno Setup Installer**: Replaced MSIX with a clean, classic Windows setup installer (`FreeRange_Exam_Suite_Setup_v3.5.exe`).
* **Zero-Lag Startup**: Optimized binary compilation (`--onedir`) eliminating temporary extraction bottlenecks.
* **Enhanced Review Export**: Updated TXT export engine to format Drag & Drop mistakes clearly.

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

### Pre-compiled Installer (Recommended)
1. Download `FreeRange_Exam_Suite_Setup_v3.5.exe` from the [Releases](../../releases) section.
2. Run the installer and select your installation directory.
3. Launch **FreeRange Exam Simulator** or **FreeRange Exam Builder** directly from the Start Menu or Desktop shortcuts.

### Running from Python Source
Ensure Python 3.10+ is installed along with Pillow:

```bash
pip install pillow

# 📄 Exam JSON File Structure & Specification (v3.5)

The **FreeRange Exam Suite** uses standard JSON files to load exam questions, properties, and exhibits. This document outlines the schema specification and provides examples for all supported question types.

---

## 🛠️ General Schema Overview

At the top level, every exam file consists of **`Properties`** (global metadata) and **`Sections`** containing an array of **`Questions`**.

```json
{
  "Properties": {
    "Title": "Exam Title",
    "ExamCode": "EXAM-CODE",
    "TimeLimit": 60,
    "Passmark": 700
  },
  "Sections": [
    {
      "Title": "General",
      "Questions": [ /* Array of Question Objects */ ]
    }
  ]
}

```

### Metadata Fields

* `Title` *(String)*: Display name of the exam.
* `ExamCode` *(String)*: Optional code (e.g., `200-301`, `SY0-701`).
* `TimeLimit` *(Integer)*: Duration of the exam in minutes.
* `Passmark` *(Integer)*: Minimum passing score out of 1000.

---

## ❓ Question Types & Definitions

An optional `"ExhibitBase64"` field containing a Base64-encoded JPEG/PNG string can be added to **any** question type to attach an image/diagram.

### 1. Single Choice

* Set `"IsMultipleChoice": false`.
* Set `"Answer"` to the single correct letter (e.g., `"A"`).

### 2. Multiple Choice

* Set `"IsMultipleChoice": true`.
* Set `"Answers"` to all correct letters concatenated (e.g., `"AC"` for options A and C).

### 3. Fill-in-the-Blank

* Set `"IsFillInTheBlank": true`.
* Place three underscores (`___`) in the `"Text"` field for every required answer.
* Define `"Blanks"` as an array containing the exact text values for each placeholder in sequence.

### 4. Drag & Drop (Matching, Ordering & Distractors)

* Set `"IsDragAndDrop": true`.
* `"Draggables"` *(Array of Strings)*: Contains all draggable items, including correct answers and optional **distractors** (extra items that don't belong to any target).
* `"Targets"` *(Array of Objects)*: Contains target slots with `"Label"` (category name or step number) and the correct `"Answer"`.

---

## 📋 Full JSON Example Specification

```json
{
  "Properties": {
    "Title": "Cisco CCNA - Full Practice Exam",
    "ExamCode": "200-301",
    "TimeLimit": 90,
    "Passmark": 825
  },
  "Sections": [
    {
      "Title": "General",
      "Questions": [

        {
          "Id": 1,
          "Topic": "Network Fundamentals",
          "Text": "Which protocol operates at the Transport Layer (Layer 4) of the OSI model?",
          "IsMultipleChoice": false,
          "Answer": "A",
          "Options": [
            { "Alphabet": "A", "Text": "TCP (Transmission Control Protocol)" },
            { "Alphabet": "B", "Text": "IP (Internet Protocol)" },
            { "Alphabet": "C", "Text": "HTTP (Hypertext Transfer Protocol)" },
            { "Alphabet": "D", "Text": "Ethernet" }
          ],
          "ExhibitBase64": "OPTIONAL_BASE64_IMAGE_STRING"
        },

        {
          "Id": 2,
          "Topic": "Network Fundamentals",
          "Text": "Select the TWO protocols that operate at the Application Layer.",
          "IsMultipleChoice": true,
          "Answers": "AC",
          "Options": [
            { "Alphabet": "A", "Text": "DNS" },
            { "Alphabet": "B", "Text": "ICMP" },
            { "Alphabet": "C", "Text": "HTTPS" },
            { "Alphabet": "D", "Text": "UDP" }
          ]
        },

        {
          "Id": 3,
          "Topic": "Wireless Fundamentals",
          "IsFillInTheBlank": true,
          "Text": "In a wireless network, the human-readable network name is the ___ while the physical MAC address of the Access Point radio is the ___ .",          "Blanks": [
            "SSID",
            "BSSID"
          ]
        },

        {
          "Id": 4,
          "Topic": "OSI Model",
          "IsDragAndDrop": true,
          "Text": "Match each Protocol Data Unit (PDU) to its corresponding OSI Layer.",
          "Draggables": [
            "Frame",
            "Packet",
            "Segment",
            "Data",
            "Bits (Unused Distractor)"
          ],
          "Targets": [
            {
              "Label": "Layer 2 - Data Link",
              "Answer": "Frame"
            },
            {
              "Label": "Layer 3 - Network",
              "Answer": "Packet"
            },
            {
              "Label": "Layer 4 - Transport",
              "Answer": "Segment"
            }
          ]
        }

      ]
    }
  ]
}

```

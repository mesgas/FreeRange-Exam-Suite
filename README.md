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
| <img src="screenshots/FreeRange%20Exam%20Suite%20(1).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(3).png" width="400"> |

| Fill-in-the-Blank Questions | Exam Results & Analytics |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(2).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(8).png" width="400"> |

| Mistakes Report | Single Choice Exhibit |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(10).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(5).png" width="400"> |

| Multiple Choice | Review Grid |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(4).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(6).png" width="400"> |

<br>

### 🛠️ Exam Builder Engine
| Builder Interface | Question Editor & DND Setup |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(11).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(14).png" width="400"> |

| Exhibit Attachment & Preview | Fill-in-the-blank |
| :---: | :---: |
| <img src="screenshots/FreeRange%20Exam%20Suite%20(15).png" width="400"> | <img src="screenshots/FreeRange%20Exam%20Suite%20(13).png" width="400"> |

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

### EXE Package (Recommended)
1. Download `FreeRange_Exam_Suite_Setup_v3.6.0.exe` from the [Releases](../../releases) section or install it directly via the **Microsoft Store**. (Certification still in progress)
2. Double-click the `.exe` file to launch the native Windows App Installer.
3. Launch **FreeRange Exam Simulator** or **FreeRange Exam Builder** directly from the Start Menu.


📄 Exam JSON File Structure & Specification (v3.6.0.0)
The FreeRange Exam Suite uses standard JSON files to load exam questions, properties, and exhibits. This document outlines the schema specification and provides examples for all supported question types.

🛠️ General Schema Overview
At the top level, every exam file consists of Properties (global metadata) and Sections containing an array of Questions.

```JSON


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

Metadata Fields
Title (String): Display name of the exam.

ExamCode (String): Optional code (e.g., 200-301, SY0-701).

TimeLimit (Integer): Duration of the exam in minutes.

Passmark (Integer): Minimum passing score out of 1000.

❓ Question Types & Definitions
An optional "ExhibitBase64" field containing a Base64-encoded JPEG/PNG string can be added to any question type to attach an image/diagram.

1. Single Choice
Set "IsMultipleChoice": false.

Set "Answer" to the single correct letter (e.g., "A").

2. Multiple Choice
Set "IsMultipleChoice": true.

Set "Answers" to all correct letters concatenated (e.g., "AC" for options A and C) or an array of strings.

3. Fill-in-the-Blank
Set "IsFillInTheBlank": true.

Place three underscores (___) in the "Text" field for every required answer.

Define "Blanks" or "Answers" as an array containing the exact text values for each placeholder in sequence.

4. Drag & Drop (Matching, Ordering & Distractors)
Set "IsDragAndDrop": true.

"Draggables" (Array of Strings): Contains all draggable items, including correct answers and optional distractors (extra items that don't belong to any target).

"Targets" (Array of Objects): Contains target slots with "Label" (category name or step number) and the correct "Answer".

📋 Full JSON Example Specification

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
          "Text": "In a wireless network, the human-readable network name is the ___ while the physical MAC address of the Access Point radio is the ___ .",
          "Blanks": [
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

⚖️ License & Legal
Copyright © 2026 mesgas (Mario Messina). All rights reserved.

FreeRange Exam Suite™, FreeRange Exam Simulator™, and FreeRange Exam Builder™ are trademarks of mesgas.
All other trademarks, product names, logos, and certification names mentioned within the application (including but not limited to Cisco®, Microsoft®, CompTIA®, AWS®, or other third-party vendor certification programs) belong to their respective owners. Their use within this software is solely for descriptive and educational purposes to identify exam compatibility and does not imply any affiliation, sponsorship, or endorsement by the trademark holders.

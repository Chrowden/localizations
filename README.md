# Chrowden's Ports Localizations

This repository contains the JSON language files used to translate the games into various languages.

# Translation Status
## Post-Shift 2
| Code | Language | Status |
| :---: | :--- | :--- |
| **EN** | **English** | 🟢 **Original Source** |
| **RU** | **Russian** | 🟢 **Manual Translation (by Chrowden)** |
| **CN** | Chinese (Simplified) | 🟠 Machine Translation (Needs Review) |
| **TW** | Chinese (Traditional)| 🟠 Machine Translation (Needs Review) |
| **DE** | German | 🟠 Machine Translation (Needs Review) |
| **ES** | Spanish | 🟠 Machine Translation (Needs Review) |
| **FR** | French | 🟠 Machine Translation (Needs Review) |
| **ID** | Indonesian | 🟠 Machine Translation (Needs Review) |
| **IT** | Italian | 🟠 Machine Translation (Needs Review) |
| **JP** | Japanese | 🟠 Machine Translation (Needs Review) |
| **KO** | Korean | 🟠 Machine Translation (Needs Review) |
| **PL** | Polish | 🟠 Machine Translation (Needs Review) |
| **PT** | Portuguese | 🟠 Machine Translation (Needs Review) |
| **TR** | Turkish | 🟠 Machine Translation (Needs Review) |
| **UA** | Ukrainian | 🟠 Machine Translation (Needs Review) |
| **VI** | Vietnamese | 🟠 Machine Translation (Needs Review) |

> Since many languages are currently machine-translated, we welcome Pull Requests from native speakers to correct errors and improve the quality of the localization.

---

# Technical Documentation

The localization files utilize specific formatting tags and a variable system for efficiency.

## 1. Text Formatting
The game engine supports Rich Text tags to style the strings. You can use the following tags within the JSON values:

| Feature | Tag Syntax | Example |
| :--- | :--- | :--- |
| **Color** | `<color=#HEXCODE>...</color>` | `This is <color=#FF0000>Red</color>` |
| **Size** | `<size=NUMBER>...</size>` | `This is <size=50>Big Text</size>` |
| **Bold** | `<b>...</b>` | `This is <b>Bold</b>` |
| **Italic** | `<i>...</i>` | `This is <i>Italic</i>` |
| **New line** | `\n` | `This is \nNew line` |

## 2. String Reuse (Variables)
To avoid repetition and ensure consistency, you can reference other strings within the same file using the `%key%` syntax.

## 3. Keep track of the length of the text
Usually, the engine is able to automatically reduce text, but sometimes it is better to use the size tag with reduced/increased font sizes. The dimensions of all the text used may be posted later...

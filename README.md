# braille-autocorrect
A Braille autocorrect system for visually impaired users
# 🧠 Braille Autocorrect System for Visually Impaired Users

**Author:** Monisha  
**Project Type:** Accessibility + NLP  
**Tech Stack:** Python, Google Colab, Levenshtein Distance, QWERTY Braille Mapping

---

## Description

This project helps **visually impaired users** input English words using **QWERTY-based Braille key combinations** like `D K` (dots 1 + 4 = letter C). It then uses **fuzzy string matching** (Levenshtein distance) and **word frequency ranking** to autocorrect mistyped Braille inputs and suggest the top 3 most likely intended words.

It supports typo-tolerant inputs and is designed to be simple, accessible, and extendable into larger assistive technology tools.

---

## Key Features

-  Accepts **space-separated Braille dot inputs** (e.g. `D K   D Q O   D K O   D O`)
-  Uses **Levenshtein distance** to handle typos
-  Ranks suggestions using **confidence score + word frequency**
-  Shows top 3 closest matches with confidence %
-  No need to type `+` or `exit` — fully accessible with keyboard/screen reader
-  Realistic for blind users using custom Braille keyboards

---

## Sample Input / Output

**Input:**
D K D Q O D K O D O

**Output:**
 code (confidence: 75%)
 cod (confidence: 75%)
 cost (confidence: 50%)

 
---

## How to Use

1. Clone or open the notebook in Google Colab
2. Run all cells
3. When prompted:
   - Type each **Braille character** as QWERTY key combos (e.g. `D Q O`)
   - Separate each Braille **letter** with **3 spaces**
   - Press Enter on empty line to exit

---

## Future Extensions

- Multi-word sentence correction
- Unicode Braille output (e.g. `⠉⠕⠙⠑`)
- Streamlit or Flask web interface
- Voice input integration

---

## Acknowledgments

- Based on Google’s 10k word list
- Inspired by assistive tech tools for screen reader and Braille users

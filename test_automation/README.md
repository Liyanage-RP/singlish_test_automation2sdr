# Singlish-to-Sinhala Transliteration Testing

This project contains automated and manual testing results for the Singlish-to-Sinhala transliteration tool provided by [Pixelssuite](https://www.pixelssuite.com/chat-translator).

**GitHub Repository:** [Liyanage-RP/singlish_test_automation2sdr](https://github.com/Liyanage-RP/singlish_test_automation2sdr)

## Files in this Repository

- **`test_automation.py`**: A Playwright-based Python script used to automate the input and extraction of transliteration results.
- **`Assignment 1 - Test cases.xlsx`**: The final test report containing 50 negative test cases across 24 linguistic categories. It includes inputs, expected outputs, actual outputs (simulated failures), and rationales.
- **`README.md`**: Project documentation.

## Test Case Overview

The test cases cover a wide range of linguistic complexities including:
- Greeting and Question forms
- English word insertions and code-mixing
- Digital terms (Wi-Fi, Laptop, etc.)
- Platform names (WhatsApp, Facebook)
- Proper nouns (Place names, Person names)
- Numeric data, Currency, and Time formats
- Long paragraph inputs

## How to Run the Automation

1. **Install Dependencies**:
   ```bash
   pip install playwright openpyxl
   playwright install chromium
   ```

2. **Execute Tests**:
   ```bash
   python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator"
   ```

*Note: Due to high latency and instability of the target web application, several tests are expected to return failures or timeouts.*

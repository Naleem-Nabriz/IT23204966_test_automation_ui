# IT3040 ITPM Assignment 1 - Option 2 Playwright Automation

This project automates one test scenario for Pixelssuite Option 2.

## Automated scenario

- Test Case ID: Pos_0036
- Feature: Image format conversion
- Website URL: https://www.pixelssuite.com/convert-to-png
- Scenario: Verify preview functionality after uploading a PNG image
- Test data: sample.png
- Expected result: The uploaded PNG file should appear in the Preview section.

## Prerequisites

Install:

1. Python 3.11 or 3.12
2. Google Chrome or Playwright Chromium

## Installation

Open Command Prompt in this folder and run:

```bash
pip install -U pip
pip install playwright openpyxl
playwright install
```

## Run the test

```bash
python image_preview_test.py --url "https://www.pixelssuite.com/convert-to-png" --slow-mo-ms 2000
```

## Expected output

After running the test, check:

1. `execution_results.csv` should contain one result row.
2. `results` folder should contain a screenshot such as `preview_pass.png`.

## Notes

If the website layout changes or the preview section does not appear within the timeout, the script may record FAIL. In that case, re-run after confirming the website is reachable and the file upload control is visible.

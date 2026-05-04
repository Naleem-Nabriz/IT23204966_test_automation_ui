# Image Preview Automation Test using Playwright

## 📌 Project Overview

This project is developed as part of the **IT3040 – IT Project Management (ITPM)** assignment.
The objective of this automation is to verify the **preview functionality** of the PNG image upload feature on the PixelsSuite website.

The test ensures that when a valid PNG image is uploaded, the system correctly displays the image in the preview section.

---

## 🌐 Tested URL

https://www.pixelssuite.com/convert-to-png

---

## ⚙️ Technologies Used

* Python 3.11 / 3.12
* Playwright (Python)
* CSV (for result logging)

---

## 📁 Project Structure

```
test_automation_ui/
│── image_preview_test.py       # Main automation script
│── execution_results.csv       # Test execution results
│── sample.png                 # Sample PNG file (auto-generated if missing)
│── results/                   # Screenshots folder
│   └── preview_pass.png
│── README.md                  # Project documentation
```

---

## ✅ Prerequisites

Before running the project, make sure you have:

* Python 3.11 or 3.12 installed
* Google Chrome (optional, Playwright can install Chromium)

---

## 🔧 Setup Instructions

### 1. Extract Project

* Download and extract the provided ZIP file to:

```
D:\test_automation_ui
```

---

### 2. Open Command Prompt

Navigate to the project folder:

```
cd /d D:\test_automation_ui
```

---

### 3. Install Dependencies

Run the following commands:

```
pip install -U pip
pip install playwright openpyxl
playwright install
```

---

## ▶️ How to Run the Test

Run the following command:

```
python image_preview_test.py --url "https://www.pixelssuite.com/convert-to-png" --slow-mo-ms 2000
```

---

## 🧪 Test Scenario Description

| Field           | Description                            |
| --------------- | -------------------------------------- |
| Feature         | Image Format Conversion (PNG Preview)  |
| Input           | Upload valid PNG file                  |
| Expected Result | Image should appear in preview section |
| Actual Result   | Preview is detected automatically      |
| Status          | PASS / FAIL                            |

---

## 📊 Output

### 1. CSV File

* File: `execution_results.csv`
* Contains:

  * File type
  * File path
  * Preview detected (True/False)
  * Status (PASS/FAIL)
  * Screenshot path

---

### 2. Screenshot

* Stored in: `results/`
* File name:

  * `preview_pass.png` (if test passes)
  * `preview_fail.png` (if test fails)

---

## ⚠️ Notes

* If `sample.png` is not available, the script automatically generates a default PNG file.
* The script detects preview by checking visible image/media elements near "Preview" labels.
* Only **one automated test scenario** is required for this assignment.

---

## 🧠 Assumptions

* The system should display a preview when a valid PNG image is uploaded.
* The preview section contains visible media elements (image/canvas/video).

---

## 📌 Conclusion

The automation script successfully verifies the preview functionality of the PNG upload feature.
Results are recorded in a CSV file and supported with a screenshot for validation.

---

Test Automation UI - Playwright Project

Project Overview

This project is developed as part of the **IT3040 – ITPM Assignment 1 (Option 2)**.
The main objective is to test the **preview functionality** of an image conversion feature available on the Pixelssuite website.

The automation is implemented using **Python** and **Playwright**, and the results are recorded in a CSV file.

---

Objective

* Verify that an uploaded PNG image is correctly displayed in the **Preview section**
* Capture execution results
* Generate a screenshot as proof
* Save results into a CSV file

---

Website Tested

https://www.pixelssuite.com/convert-to-png

---

Technologies Used

* Python 3.11 / 3.12
* Playwright
* OpenPyXL
* CSV for result storage

---

Project Structure

```
test_automation_ui/

 image_preview_test.py          # Main automation script
 sample.png                     # Sample test image
 execution_results.csv          # Output results file
 results/
      preview_pass.png           # Screenshot of successful execution
```

---

Setup Instructions

Install Prerequisites

* Install Python (3.11 or 3.12)
* Install Google Chrome (optional)

---

Install Dependencies

Open Command Prompt and navigate to the project folder:

```
cd /d D:\test_automation_ui
```

Run the following commands:

```
pip install -U pip
pip install playwright openpyxl
playwright install
```

---

Configuration

Open the file:

```
image_preview_test.py
```

Find this line:

```
DEFAULT_URL = "https://www.pixelssuite.com/image-to-pdf"
```

Change it to:

```
DEFAULT_URL = "https://www.pixelssuite.com/convert-to-png"
```

Save the file.

---

How to Run the Test

Run the following command:

```
python image_preview_test.py --url "https://www.pixelssuite.com/convert-to-png" --slow-mo-ms 2000
```

---

Output

After execution:

CSV File

* File: `execution_results.csv`
* Contains:

  * file_type
  * file_path
  * preview_detected
  * status
  * screenshot path

---

Screenshot

* Location: `results/preview_pass.png`
* Used as proof of successful preview detection

---

Expected Result

* The uploaded PNG image should be displayed in the Preview section
* Status should be recorded as **PASS**
* Screenshot should be generated

---

Test Scenario Automated

**Feature:** Image Format Conversion (PNG)

**Test Type:** Positive Test Case

**Description:**
Upload a valid PNG image and verify that it appears in the Preview section.

---

Submission Files

* Playwright project folder
* execution_results.csv
* Manual test cases Excel file
* Git repository link

---

Repository Link - https://github.com/Pirakash12/Test_Automation_UI.git

---

Author

* Registration Number: IT23312876

---

Notes

* Ensure the repository is **public**
* Do not modify the CSV structure
* Only one automation scenario is required

---

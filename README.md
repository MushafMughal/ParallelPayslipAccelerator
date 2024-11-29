# PaySlip-Generator
This project automates the generation of payslips for employees in your company using a web automation script. It processes employee data from an Excel file, fills in the necessary fields on a payslip generator website, and downloads the payslips as PDF files. The system can generate approximately **100 payslips in around 6 minutes**, significantly reducing manual effort and time.
### Features
 - **Automated Data Input:** Reads employee details and payroll information from an Excel file.
 - **Dynamic Web Interaction:** Interacts with the web application to populate fields for employee details, earnings, and deductions.
 - **Payslip Download:** Downloads the payslips in PDF format and saves them with descriptive filenames.
 - **Efficient Processing:** Handles large volumes of data quickly and accurately.
 - **Customizable Fields:** Supports customization for earnings and deduction fields.
# How It Works
### 1. Data Preprocessing:
 - Reads employee details from Demo.xlsx.
 - Converts specific columns to the required formats (e.g., dates and numeric values).
### 2. Web Interaction:
 - Opens the Free Payslip Generator[printyourcopy.com/free-payslip-generator] in Microsoft Edge.
 - Uploads the company logo and enters static company details.
 - Customizes earning and deduction field descriptions.

### 3. Payslip Generation:
 - Iterates through each row in the employee data file.
 - Fills in the payslip fields for employee details, earnings, and deductions.
 - Downloads and renames each payslip based on the employee’s name and the month.
### 4. Cleanup:
 - Clears the fields after each payslip generation to prepare for the next entry.
# Key Functions in the Script
  1. **data_preprocessing(file_path)**
     Reads and preprocesses the Excel file for correct data formatting.

  2. **setup_static_details()**
     Configures the static fields on the payslip generator, such as the logo, employer details, and custom fields.

  3. **update_field_descriptionss(descriptions, category)**
     Updates the descriptions for earnings and deductions fields dynamically.
  4. **process_payslips()**
     Processes each employee's details, generates payslips, and organizes them into the output directory.
# Performance
 - Generates 100 payslips in approximately 6 minutes.
 - Automates repetitive tasks with minimal human intervention.
 - Ensures consistency and accuracy in payslip creation.
# Environment
 - **Python:** Version 3.12.5
 - **Selenium:** Version 4.27.0
 - **Pandas:** Version 2.2.2
 - **Edge WebDriver:** Version 131.0.2903.70 (Ensure compatibility with the version of Microsoft Edge installed on your system.)

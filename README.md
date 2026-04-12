# Medicalappointmentt
Data Cleaning and preprocessing
Overview

This project involves cleaning and preprocessing a raw CSV dataset using Microsoft Excel to ensure data consistency, accuracy, and usability for further analysis and visualization.

Steps Performed
Opened Raw Dataset
Imported the raw .csv file into Microsoft Excel.

Verified Column Headings
Checked all column names for correctness and consistency.

Renamed columns where necessary to maintain a uniform format.

Removed Duplicate Rows
Used Excel’s built-in feature:

Data → Remove Duplicates

Ensured only unique records were retained.

Removed Blank Rows
Applied filters to identify blank rows.

Deleted rows where key fields were empty.

Trimmed Extra Spaces
Removed leading and trailing spaces using:

=TRIM(A2)

Applied across all relevant text columns.

Standardised Categorical Values
Ensured consistent naming (e.g., "Male", "male", "M" → "Male").

Used:

=UPPER(A2)

or

=PROPER(A2)

Applied Find & Replace where needed.

Processed Date Columns
Converted text dates into proper Excel date format using:

=DATEVALUE(A2)

Applied custom formatting:

Format Cells → Date

Split Date and Time Columns
For columns like ScheduledDay and AppointmentDay:

Extracted Date:

=INT(A2)

Extracted Time:

=MOD(A2,1)

Formatted:

Date → Date format

Time → Time format

Saved Cleaned Dataset
Saved the processed file as a new Excel file:

File → Save As → .xlsx

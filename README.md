# SpreadsheetCellInverter.py

**Spreadsheet Cell Inverter Code Analysis**

**Purpose:** This Python script inverts the cell values of a spreadsheet by transposing its rows and columns.

**Description:**

1. The script loads an Excel workbook named "Inverse.xlsx" using the `openpyxl` library.
2. It selects the active sheet from the workbook.
3. A new workbook is created using `openpyxl.Workbook()`.
4. The active sheet from the new workbook is selected.
5. The script iterates over each column (using `range(sheet.max_column)`) and row (using `range(sheet.max_row)`) of the original sheet.
6. For each cell, it assigns the value from the original sheet to the corresponding cell in the new sheet, but with the row and column indices swapped.
7. Finally, the script saves the new workbook as "Inverse_copy.xlsx".

**Example Use Case:**

Suppose you have a spreadsheet with data in the following format:

| A |
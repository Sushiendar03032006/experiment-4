# AIM:
To read data from one Excel file and write it into another Excel file using UiPath.

# Software Required:
```
1.UiPath Studio
2.xlsx Excel files (source and destination)
```

# Procedure:
# 1. Open UiPath Studio:
  Create a new process or open an existing one.
# 2. Declare DataTable Variable:
  Create a variable named dtFilteredData of type DataTable to store the data read from Excel.
# 3. Read Data from Source File:
    Activity: Read Range Workbook
    File Path: C:\Users\msush\OneDrive\Documents\exceloperationsuipath.xlsx
    Sheet Name: "Sheet1"
    Range: "" (blank to read the full sheet)
    Output: dtFilteredData
    Add Headers: Checked
# 4. Write Data to Destination File:
     Activity: Write Range Workbook
     File Path: C:\Users\msush\OneDrive\Desktop\invoice.xlsx
     Sheet Name: "Sheet1"
     Range: "A1" (start writing from the first cell)
     Input DataTable: dtFilteredData
     Add Headers: Checked ✅

## Workflow:
![Screenshot 2025-05-05 224400](https://github.com/user-attachments/assets/3e9ed659-7e5b-429e-8b7a-b2cbdb0162d7)

## Output:
![image](https://github.com/user-attachments/assets/b8986c4d-af46-4eab-a18a-034f89591edc)


## Result:
```
The data from exceloperationsuipath.xlsx is successfully read.
It is then written to the invoice.xlsx file starting from cell A1, including the headers.
```



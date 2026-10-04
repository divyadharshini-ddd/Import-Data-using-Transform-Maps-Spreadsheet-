# Import-Data-using-Transform-Maps-Spreadsheet-
Import Data Using Transform Maps is a ServiceNow process used to import data from Excel or CSV files into a target table. A Transform Map connects spreadsheet fields with ServiceNow fields. It helps map, validate, transform, insert, and update data accurately. After importing, the records are verified in the target table.
README

Import Data Using Transform Maps (Spreadsheets)

Table of Contents

1. Introduction
2. Objective
3. Prerequisites
4. Understanding Import Sets
5. Understanding Transform Maps
6. Spreadsheet Data Preparation
7. Importing Spreadsheet Data
8. Creating a Transform Map
9. Field Mapping
10. Data Transformation
11. Running the Transform
12. Verification and Validation
13. Expected Result
14. Advantages
15. Conclusion

---

1. Introduction

Import Data Using Transform Maps (Spreadsheets) is a process used to import data from spreadsheet files such as Excel or CSV into a target table in ServiceNow.

The Import Set collects the data from the spreadsheet, while the Transform Map determines how the imported data should be transferred and mapped to the fields of the target table.

This process is useful when a large amount of data needs to be added to the system without entering each record manually.

---

2. Objective

The main objectives of this process are:

- To import data from a spreadsheet into ServiceNow.
- To understand the concept of Import Sets and Transform Maps.
- To map source fields with target table fields.
- To transform and validate data during the import process.
- To efficiently handle bulk data insertion or updating.

---

3. Prerequisites

Before performing the import, the following requirements are needed:

- A ServiceNow instance.
- An Excel or CSV spreadsheet containing the required data.
- Access to the Import Set functionality.
- A suitable target table.
- Proper field names and values in the spreadsheet.

---

4. Understanding Import Sets

An Import Set is used as a temporary staging area for data imported from external sources such as spreadsheets.

When a spreadsheet is uploaded, its data is first loaded into an Import Set table. The data can then be processed and transferred to the required target table using a Transform Map.

---

5. Understanding Transform Maps

A Transform Map defines how data from an Import Set should be transferred to a target table.

It specifies the relationship between the source fields and target fields. Transform Maps can also contain transformation logic to modify or validate data before it is inserted into the target table.

---

6. Spreadsheet Data Preparation

Before uploading the spreadsheet, the data should be properly organized.

The spreadsheet should contain:

- Column headings.
- Valid data values.
- No unnecessary blank rows.
- Correct data formats.
- Unique values where required.

Example:

Employee ID| Name| Department| Email
E101| Arun| IT| arun@example.com
E102| Priya| HR| priya@example.com
E103| Kumar| Finance| kumar@example.com

---

7. Importing Spreadsheet Data

The spreadsheet is uploaded into ServiceNow through the Import Set functionality.

The system reads the spreadsheet and creates records in a temporary Import Set table. These records are then ready to be transformed into the required target table.

---

8. Creating a Transform Map

After importing the spreadsheet:

1. Open the Import Set.
2. Select the appropriate Import Set table.
3. Create a new Transform Map.
4. Select the required target table.
5. Save the Transform Map.
6. Configure the required field mappings.

The Transform Map acts as a bridge between the imported data and the target table.

---

9. Field Mapping

Field mapping specifies which source field should be transferred to which target field.

Example:

Source Field| Target Field
Employee ID| Employee ID
Name| Name
Department| Department
Email| Email

Correct field mapping ensures that the imported information is stored in the appropriate fields.

---

10. Data Transformation

Data transformation allows the imported values to be modified before they are stored in the target table.

For example, a transformation can:

- Change the format of a value.
- Convert text into another format.
- Set default values.
- Validate imported information.
- Perform calculations.
- Clean unwanted data.

This helps maintain data quality and consistency.

---

11. Running the Transform

After configuring the Transform Map, the transformation process is executed.

During this process:

Spreadsheet → Import Set Table → Transform Map → Target Table

The Transform Map processes the imported records and transfers them to the target table according to the configured mappings and transformation rules.

---

12. Verification and Validation

After the transformation is completed, the target table should be checked to verify that:

- All required records are imported.
- Fields contain the correct values.
- No important records are missing.
- Data is stored in the correct format.
- Any errors or rejected records are identified and corrected.

---

13. Expected Result

The spreadsheet data should be successfully imported into the selected target table.

The source fields should be correctly mapped to their corresponding target fields, and any configured transformation rules should be applied successfully.

---

14. Advantages

- Bulk Data Import: Large amounts of data can be imported at once.
- Time Saving: Reduces manual data entry.
- Data Mapping: Provides proper mapping between source and target fields.
- Data Transformation: Allows data to be modified during import.
- Data Accuracy: Helps maintain consistency in imported records.
- Easy Management: Makes data migration and updating easier.

---

15. Conclusion

Importing data using Transform Maps and spreadsheets is an efficient method for transferring bulk data into ServiceNow. Import Sets provide a temporary location for the uploaded data, while Transform Maps control how the data is mapped and transformed before being stored in the target table.

This process improves efficiency, reduces manual work, and helps maintain accurate and consistent data within the system.

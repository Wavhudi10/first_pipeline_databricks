# CRM

## Customer Information

The customer information table was reviewed in collaboration with the bootcamp instructor. The cleaning process focused on identifying and removing empty spaces, resolving abbreviations, and renaming columns to more descriptive, readable names.

---

## Product Information

### Duplicate Check
No duplicate records were found. The product ID column was used as the unique identifier to validate this.

### String Validation
All text columns were trimmed to remove leading and trailing whitespace. The product line column was found to contain abbreviated values and was normalised to full descriptive labels.

### Date Validation
Date columns were confirmed to be in the correct data type and format (`YYYY-MM-DD`). Null values in the product end date column are expected and valid, as they indicate products without a defined end date.

A date integrity issue was identified where several end dates preceded their corresponding start dates. Investigation revealed that the years 2011 and 2012 had been incorrectly recorded as 2007 and 2008 respectively. This was corrected by adding six years to the affected end dates.

### Numeric Validation
The product cost column was found to contain null values, which were flagged and handled as part of the cleaning process.

### Business Key Standardisation
To ensure accurate joins across tables, the product key column was standardised by extracting only the first four characters, aligning it with the matching ID format used in the corresponding ERP category table.

### Column Renaming
All column names were renamed to more readable and business-friendly labels.

to be continued ...
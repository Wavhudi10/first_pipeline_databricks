# CRM

###crm_cust_info 
- This was done with the instructor on bootcamp identified empty spaces, abbreviations, renamed coluns to better names

###crm_prd_inf
- No duplicates where found, used prd_id to check
- validating string values
  - Checking empty spaces
      - we found the prd_line columns cotaining.
      - we will TRIM all text columns
  - Identifying abbreviations to normalise:
    - column prd_line is in abreviations.
- validating dates
  - Data type - correct data type
  - format also correct year-month-date
  - handling missing value - prd_end_dt has null values but that is okay as it is showing that the end date been reached.
  - The is date error the end date is before the start date
    - upon checking the data year 2011 was replaced by 2007 and year 2012 was replaced by 2008. we will add the 6 years to the end dates.
- validating numeric values
  - product cost has nulls
- Standadising business key IDs to ensure tables are joined correctly
  - we will use the first 4 chracters of the prd_key column as it matches the ID of table erp_px_cat_g1v2raw
- we will rename our columns to something more freindly
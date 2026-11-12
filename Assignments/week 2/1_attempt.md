# Assignment 2: Step 1 - Manual Diagnosis & Attempt
## Dataset Overview
- **File Audited:** `teaching_prices_messy.csv`
- **Total Records:** 97 rows, 6 columns (`date`, `item`, `city`, `price`, `unit`, `data_label`)

## Identified Issues & Planned Decisions
1. **Missing Value (`NaN`)**
   - **Detection:** Checked missing values via column null counts (`df.isnull().sum()`). Found 1 missing price in Row 5 (`2026-01-01`, `Pulse C`, `City 2`).
   - **Planned Decision:** Investigate — Will determine whether to impute using median/mean price for Pulse C in City 2 or flag it for exclusion.

2. **Formatting Error (Comma in Number)**
   - **Detection:** Inspected unique price values; caught text-formatted string `'1,250'` instead of a float in Row 17 (`2026-01-15`, `Staple A`)
   - **Planned Decision:** Correct — Remove the comma and cast the column/value to numeric float.

3. **Extreme Outlier**
   - **Detection:** Scanned high-range price values and found `9999` in Row 30 (`2026-01-22`, `Sweetener D`, `City 1`).
   - **Planned Decision:** Exclude — This is an unrealistic outlier for this commodity and should be treated as bad data or dropped.

4. **Exact Duplicate Row**
   - **Detection:** Checked duplicated rows based on primary keys (`date`, `item`, `city`) and found Row 96 duplicating.
   - **Planned Decision:** Exclude — Drop duplicate entry to avoid double-counting.

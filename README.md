# URT_NSCL

## Dataset Overview

| Sample ID                 | RP11.34P13.3 | RP11.34P13.7 | ... | Diagnosis |
|---------------------------|---------------|---------------|-----|-----------|
| F00431_AGAGCTTGTAGAGGAA   | 0             | 0             | ... | IPF       |
| F01380_GATCTAGTCTTGCCGT   | 0             | 0             | ... | IPF       |
| Sample_3_ID               | 1.23          | 0.45          | ... | Control   |
| Sample_4_ID               | 2.34          | 1.78          | ... | IPF       |


## Dataset Description

### Columns

#### Gene Identifiers (e.g., RP11.34P13.3, FO538757.3, etc.)
- Each column (except the last) represents a **gene**, identified by names such as `RP11.34P13.3`, `FO538757.3`, etc.
- The values under these columns are numeric (`<dbl>`), representing the **gene expression levels**.
  - These values are likely **counts** or **normalized** measures (e.g., log-transformed counts).
  
#### Diagnosis (Classification Label)
- The last column, `Diagnosis`, contains the classification **label** for each sample.
- It indicates whether the sample belongs to the **"IPF"** (Idiopathic Pulmonary Fibrosis) or **"Control"** group.
- Data type: `<chr>` (character/string).

---

### Rows (Sample Identifiers)

#### Sample Identifiers (e.g., F00431_AGAGCTTGTAGAGGAA, F01380_GATCTAGTCTTGCCGT)
- Each row corresponds to an individual **sample**, which could represent a **cell** (scRNA-seq) or a **bulk RNA-seq** sample.
- Identifiers like `F00431_AGAGCTTGTAGAGGAA` are unique for each sample:
  - `F00431`: **Sample or batch ID**.
  - `AGAGCTTGTAGAGGAA`: **Unique molecular barcode** to identify the cell or RNA molecule.

#### Gene Expression Values
- For each sample, the numeric values in the gene columns represent the **expression levels** of those genes.
- In the example shown, many values are `0`, indicating **no detectable expression** for the displayed genes in those specific samples.

---

# Executive Sales and Operations - Power BI Dashboard

Interactive Power BI report for chocolate shipments with executive KPIs like Net Sales, Gross Margin %, On-Time %, OTIF %, and Lead Time. 
Built using a star schema with 1 fact and 4 dimensions.

**Report**: `dashboard/Executive sales and operations dashboard.pbix`  
**Data**: `data/sample-chocolate-shipments-data-all-Apr-2025.xlsx`

## Highlights - your work
- Modeled the dataset as a star schema and documented relationships.
- Power Query to normalize Excel into Fact and Dimensions with surrogate keys.
- DAX for Sales, Margin, On-Time, OTIF, and YoY trend analysis.
- Performance tweaks: hidden technical columns and single direction relationships.

## Schema
See `docs/modeling.md` for the diagram and notes.

## How to open
1) Open the PBIX file.  
2) Update the Excel path to the file in `data/` if needed.  
3) Refresh the report.

## Repository structure
```
powerbi-chocolate-shipments/
├─ README.md
├─ dashboard/
│  └─ Executive sales and operations dashboard.pbix
├─ data/
│  └─ sample-chocolate-shipments-data-all-Apr-2025.xlsx
├─ docs/
│  ├─ data_dictionary.md
│  ├─ modeling.md
│  ├─ dax_measures.md
│  └─ HOWTO.md
└─ images/
   ├─ sheets in PDF
```

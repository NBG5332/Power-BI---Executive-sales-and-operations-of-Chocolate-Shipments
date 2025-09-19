# DAX Measures (adjust to your column names)
```
Total Orders = DISTINCTCOUNT(FactShipments[OrderID])
Total Units = SUM(FactShipments[Quantity])
Net Sales = SUM(FactShipments[Sales])
COGS = SUM(FactShipments[Cost])
Gross Margin = [Net Sales] - [COGS]
Gross Margin % = DIVIDE([Gross Margin], [Net Sales])

On-Time Shipments = CALCULATE(COUNTROWS(FactShipments), FactShipments[OnTimeFlag] = 1)
On-Time % = DIVIDE([On-Time Shipments], [Total Orders])
Avg Lead Time (Days) = AVERAGE(FactShipments[LeadTimeDays])
OTIF % = DIVIDE(CALCULATE(COUNTROWS(FactShipments), FactShipments[OTIF_Flag] = 1), [Total Orders])

Net Sales LY = CALCULATE([Net Sales], DATEADD(DimDate[Date], -1, YEAR))
Net Sales YoY % = DIVIDE([Net Sales] - [Net Sales LY], [Net Sales LY])

Avg Price per Unit = DIVIDE([Net Sales], [Total Units])
```

# Data Modeling (Star Schema)

Sales and operations data modeled as a **star schema**.

## Tables
- **FactShipments**: one row per order or shipment line with measures like Quantity, Sales, Cost, Margin, LeadTimeDays, OnTimeFlag, OTIF_Flag.
- **DimDate**: ['Shipdate']
- **DimProduct**: ['Product', 'SKU', 'Category']
- **DimCustomer**: ['Customer', 'Account']
- **DimGeography**: ['Country', 'Region', 'State', 'City']
- **DimLogistics** (optional): ['ShipmentID', 'Shipdate']

## Relationships
```
DimDate      (DateKey)      1 - * (DateKey)      FactShipments
DimProduct   (ProductKey)   1 - * (ProductKey)   FactShipments
DimCustomer  (CustomerKey)  1 - * (CustomerKey)  FactShipments
DimGeography (GeoKey)       1 - * (GeoKey)       FactShipments
[DimLogistics (LogisticsKey) 1 - * (LogisticsKey) FactShipments]
```

## Power Query guidance
- Promote headers, set types, trim and clean text.
- Build dimensions by taking **DISTINCT** of their attributes, add surrogate keys.
- Build fact by keeping numeric measures and foreign keys to dimensions.
- Mark **DimDate** as date table. Prefer single direction relationships.

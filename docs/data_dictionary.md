# Data Dictionary

| Sheet          |   Rows |   Cols |
|:---------------|-------:|-------:|
| Shipments      |  25076 |      8 |
| Dimension Data |     27 |     16 |
| Calendar       |    822 |      7 |

---

| Sheet          | Field        | Dtype          |   Nulls |   Unique |
|:---------------|:-------------|:---------------|--------:|---------:|
| Shipments      | ShipmentID   | object         |       0 |    25076 |
| Shipments      | SPID         | object         |       0 |       25 |
| Shipments      | PID          | object         |       0 |       22 |
| Shipments      | GID          | object         |       0 |        6 |
| Shipments      | Shipdate     | datetime64[ns] |       0 |      586 |
| Shipments      | Amount       | float64        |       0 |     6378 |
| Shipments      | Boxes        | int64          |       0 |     1627 |
| Shipments      | Order_Status | object         |       0 |        4 |
| Dimension Data | Unnamed: 0   | float64        |      27 |        0 |
| Dimension Data | Unnamed: 1   | object         |       4 |       23 |
| Dimension Data | Unnamed: 2   | object         |       4 |        4 |
| Dimension Data | Unnamed: 3   | object         |       4 |       23 |
| Dimension Data | Unnamed: 4   | object         |       4 |       23 |
| Dimension Data | Unnamed: 5   | float64        |      27 |        0 |
| Dimension Data | Unnamed: 6   | float64        |      27 |        0 |
| Dimension Data | Unnamed: 7   | object         |      20 |        7 |
| Dimension Data | Unnamed: 8   | object         |      20 |        4 |
| Dimension Data | Unnamed: 9   | object         |      20 |        7 |
| Dimension Data | Unnamed: 10  | float64        |      27 |        0 |
| Dimension Data | Unnamed: 11  | float64        |      27 |        0 |
| Dimension Data | Unnamed: 12  | object         |       1 |       26 |
| Dimension Data | Unnamed: 13  | object         |       1 |        5 |
| Dimension Data | Unnamed: 14  | object         |       1 |       26 |
| Dimension Data | Unnamed: 15  | object         |       1 |       26 |
| Calendar       | Unnamed: 0   | float64        |     822 |        0 |
| Calendar       | Unnamed: 1   | object         |       0 |      822 |
| Calendar       | Unnamed: 2   | object         |       0 |       13 |
| Calendar       | Unnamed: 3   | object         |       0 |       13 |
| Calendar       | Unnamed: 4   | object         |       0 |        4 |
| Calendar       | Unnamed: 5   | object         |       0 |        8 |
| Calendar       | Unnamed: 6   | object         |       0 |        8 |
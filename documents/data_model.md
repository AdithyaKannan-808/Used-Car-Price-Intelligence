##  Data Model (Star Schema)

**FACT_Car**  
Contains listing-level details including price, mileage, car age, fuel type, transmission, seats, and ML-predicted price (via Index join).

**Dimensions**
- **Dim_Fuel**
- **Dim_Transmission**
- **Dim_Age**
- **Dim_KMGroup**
- **Dim_PriceBand**

All tables are connected in a clean star schema. Data was prepared in **Power Query** with:
- Type cleaning  
- Numeric extraction (e.g., *“1197 cc” → 1197*)  
- Banding logic for age, price, and mileage  

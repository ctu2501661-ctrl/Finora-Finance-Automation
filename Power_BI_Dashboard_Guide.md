# Power BI Dashboard Guide — Finora
1. Open Power BI Desktop and choose Get Data → Text/CSV.
2. Import `Finora_Finance_Sales_Dataset.csv`.
3. Confirm Date is Date, Leads and Conversions are Whole Number, and value fields are Decimal/Whole Number.
4. Create measures:
   - Total Leads = SUM(Data[Leads])
   - Total Conversions = SUM(Data[Conversions])
   - Conversion Rate = DIVIDE([Total Conversions],[Total Leads],0)
   - Potential Value = SUM(Data[Potential_Value_INR])
5. Suggested visuals:
   - KPI cards: Total Leads, Total Conversions, Conversion Rate
   - Clustered column: Leads by Region
   - Bar chart: Conversions by Product
   - Donut: Leads by Marketing Channel
   - Line chart: Leads by Date
6. Add slicers for Region, Product and Marketing_Channel.
7. Label the report as a student demonstration using synthetic data.

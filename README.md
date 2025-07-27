An interactive Power BI dashboard analyzing coffee sensory data from the Coffee Quality Institute.
📝 Project Overview

This report helps stakeholders understand what drives coffee cup quality across:

- **Sensory Attributes** (Acidity, Aroma, Flavor, Body, Sweetness, etc.)  
- **Defect Categories** (Category One & Two Defects)  
- **Geography** (Country of Origin, Region)  
- **Processing Methods**  

It also incorporates a **What‑If Parameter** to model score adjustments, and an AI‑powered **Q&A** visual for self‑service insights.

## 🚀 Features

1. **Model & Data Prep**  
   - Data imported via Power Query  
   - Relationships defined between sensory, defects & metadata tables  

2. **DAX Measures**  
   - `Average_CupPoints = AVERAGE('Data'[Total_Cup_Points])`  
   - `Total_Defects = SUM('Data'[Category_One]) + SUM('Data'[Category_Two])`  
   - `Adjusted_Points = [Value] + 'Value_Adjustment'[Value]`  

3. **Pages**  
   - **Key Determinants**: Stacked bars by Cup Quality Category  
   - **Quality Scores**: Scatter & regional bar charts  
   - **Defect Trends**: Line chart with tooltips  
   - **What‑If Analysis**: Simulation of score adjustments  
   - **Overall Quality**: Country & variety comparisons  
   - **Tooltips & Q&A**: Enhanced user experience  

4. **Interactivity**  
   - Slicers for Harvest Year, Grading Date, Country, Processing Method, Color, etc.  
   - Bookmarks & buttons for guided navigation  
   - AI‑powered Q&A with synonyms 

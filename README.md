# 📊 ExcelProject
Data analysis projects using Excel – starting with the Kaggle Medical Insurance Cost dataset.

---

## 🛠 My Process (with snapshots)

I like keeping things clean and step-by-step, so here’s what I did:

1. **Duplicate the data sheet**  
   - Always keep a safe copy of the original dataset before making any changes.  
   ![Create Duplicate](https://github.com/hadishokri11/ExcelProject/blob/main/1st%20Duplicate%20data.png?raw=true)

2. **Convert data to Excel Tables + Power Query**  
   - Changed data types properly (numbers, text, categories).  
   - Ran **descriptive stats** with ToolPak to get a quick summary 👇  


## 🔍 Descriptive Analysis (Excel ToolPak)
   ![Descriptive Stats](https://github.com/hadishokri11/ExcelProject/blob/main/2nd%20Clean%20&%20Prep%20the%20Data.PNG?raw=true)
   
Before diving into pivots and regressions, I ran a **descriptive stats report** using Excel’s ToolPak.  
This gave me a quick look at the basics for each column:

- **Age** → Avg around mid-30s, range from 18 to 64.  
- **BMI** → Centered around 30 (with some pretty high outliers 👀).  
- **Children** → Most people had 0–2 kids.  
- **Charges** → Very skewed! A few people had insanely high medical costs.  

3. **PivotTables + BMI Bins**  
   - Built PivotTables for quick exploration.  
   - Added weight class bins for BMI (Normal, Overweight, Obese).  


## 📊 PivotTable Fun
   ![Pivot](https://github.com/hadishokri11/ExcelProject/blob/main/3rd%20Pivot.PNG?raw=true)  

Some quick findings from the pivots:

- 🚬 There are more **male smokers** than female smokers.  
- 🏋️ Higher **BMI groups** = way higher charges (obese patients pay a lot more).  
- 🎂 When you group ages, you see costs climb steadily as people get older.  
- 👨‍👩‍👧 Number of kids doesn’t seem to change costs that much.  
- 🌍 Region doesn’t make a big difference (so I’ll probably drop it later).  

Cool thing about PivotTables is how easy it is to mix categories — like seeing charges for *smokers + BMI groups* together. That’s where you see obese smokers shooting the costs through the roof 🚀.  

4. **Correlation Matrix + Scatter Plots**
   - Ran a correlation matrix using Excel’s ToolPak.
   - Verified relationships with scatter plots (charges vs age, BMI, smoker status).
     
##🔗 Correlation Analysis (Excel Scatter plot & ToolPak)
![Correlation](https://github.com/hadishokri11/ExcelProject-HealthCharges/blob/main/4th%20Corelation.PNG?raw=true)

I also ran a correlation matrix using Excel’s ToolPak to see which factors are most related to charges:

- Smoker vs Charges → 0.79 💥 strongest relationship by far. Being a smoker massively drives up costs.
- Age vs Charges → 0.30 → moderate link, older people tend to pay more.
- BMI vs Charges → 0.20 → weak, but noticeable. Higher BMI means slightly higher charges.
- Children vs Charges → 0.07 → almost no effect.

So smoking is the big one 🚬🔥, followed by age, then BMI. Kids and region don’t really matter much here.

To double-check, I also added scatter plots (e.g., charges vs age, charges vs BMI) — the patterns matched the correlations:

- Clear upward trend for age vs charges.
- Smokers vs non-smokers split into two very different cost clusters.
- BMI vs charges shows a weak upward spread with some outliers.




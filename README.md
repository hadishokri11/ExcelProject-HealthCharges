# 📊 ExcelProject
Data analysis projects using Excel – starting with the Kaggle Medical Insurance Cost dataset.

---

## 🛠 My Process (with snapshots)

I like keeping things clean and step-by-step, so here’s what I did:

1. **Duplicate the data sheet**  
   - Always keep a safe copy of the original dataset before making any changes.  
   [Create Duplicate](https://github.com/hadishokri11/ExcelProject/blob/main/1st%20Duplicate%20data.png?raw=true))  

2. **Convert data to Excel Tables + Power Query**  
   - Changed data types properly (numbers, text, categories).  
   - Ran **descriptive stats** with ToolPak to get a quick summary.  
   [Descriptive Stats](images/step2_toolpak.png)  

3. **PivotTables + BMI Bins**  
   - Built PivotTables for quick exploration.  
   - Added weight class bins for BMI (Normal, Overweight, Obese).  
   ![BMI Bins Pivot](images/step3_pivot_bmi.png)  

---

## 🔍 Descriptive Analysis (Excel ToolPak)

Before diving into pivots and regressions, I ran a **descriptive stats report** using Excel’s ToolPak.  
This gave me a quick look at the basics for each column:

- **Age** → Avg around mid-30s, range from 18 to 64.  
- **BMI** → Centered around 30 (with some pretty high outliers 👀).  
- **Children** → Most people had 0–2 kids.  
- **Charges** → Very skewed! A few people had insanely high medical costs.  

---

## 📊 PivotTable Fun

Some quick findings from the pivots:

- 🚬 There are more **male smokers** than female smokers.  
- 🏋️ Higher **BMI groups** = way higher charges (obese patients pay a lot more).  
- 🎂 When you group ages, you see costs climb steadily as people get older.  
- 👨‍👩‍👧 Number of kids doesn’t seem to change costs that much.  
- 🌍 Region doesn’t make a big difference (so I’ll probably drop it later).  

Cool thing about PivotTables is how easy it is to mix categories — like seeing charges for *smokers + BMI groups* together. That’s where you see obese smokers shooting the costs through the roof 🚀.  

---

## 🚀 Next Steps

- Add regression analysis with ToolPak.  
- Rebuild the same project in Python (Pandas + Scikit-learn).  
- Compare Excel vs Python results.  

---
This way your README reads like a story of your process, with snapshots showing progress.

👉 Do you want me to also make a cleaner dashboard layout suggestion (so your PivotTables + charts look polished when you screenshot them)?







You said:
Can ypu fit the description to my step to step


ChatGPT said:
Got it 👍 Let’s make the README description flow step by step with your exact process (duplicate → clean with Power Query → descriptive stats → PivotTables with BMI bins). I’ll keep it casual, like you wanted.

markdown
Copy code
# 📊 ExcelProject
Data analysis projects using Excel – starting with the Kaggle Medical Insurance Cost dataset.

---

## 🛠 My Step-by-Step Process

### 1️⃣ Duplicate the Data Sheet
First thing I did was **make a copy of the original dataset**.  
That way the raw data stays safe, and I can mess around on the duplicate without worry.  
![Original + Clean Sheet](images/step1_duplicate.png)

---

### 2️⃣ Clean & Prep the Data
- Converted the dataset into an **Excel Table** for easier handling.  
- Used **Power Query** to fix data types (numbers → numeric, text → categorical).  
- Ran a **descriptive stats report** with ToolPak to get a feel for the data:  
  - **Age** → Avg mid-30s, range 18–64.  
  - **BMI** → Centered around 30, with some big outliers 👀.  
  - **Children** → Most people had 0–2.  
  - **Charges** → Very skewed (a few very high costs).  

![Descriptive Stats](images/step2_toolpak.png)

---

### 3️⃣ Explore with PivotTables
Once the data was clean, I built **PivotTables** to explore relationships.  
I also added **BMI bins** (Normal, Overweight, Obese) to make comparisons clearer.  

Some findings so far:  
- 🚬 More **male smokers** than female smokers.  
- 🏋️ Higher **BMI groups** = way higher charges.  
- 🎂 Costs rise steadily with age groups.  
- 👨‍👩‍👧 Number of kids doesn’t change much.  
- 🌍 Region doesn’t really matter.  

![BMI Bins Pivot](images/step3_pivot_bmi.png)

---

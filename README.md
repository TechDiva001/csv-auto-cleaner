# 🧹 CSV Auto-Cleaner

> Built by Benedicta Bondzie | The Tech Diva

I am a solo learner publicly documenting my full journey into AI/ML engineering from scratch.

This project is my **Phase 1 Capstone** — built after completing Statistics, EDA, and Visualization as part of my structured self-taught AI/ML roadmap.

If you want to follow the journey, see the struggles, the projects, and the progress in real time:
👉 [the-tech-diva-aiml-journey](https://github.com/TechDiva001/the-tech-diva-aiml-journey) — give it a ⭐ if it inspires you.

---

## 📌 What Is This?

The CSV Auto-Cleaner is an interactive, step-by-step data cleaning tool built in Python and designed to run on **Google Colab**.

You upload any messy CSV file. The tool walks you through every cleaning decision. Missing values, duplicates, outliers, data types and at the end you download a clean, analysis-ready dataset. 

No code to write. Just run each cell and follow the prompts.

---

## ⚠️ Google Colab Only

This notebook only works on **Google Colab**. The file upload, interactive prompts, and download step all depend on the Colab environment. It will not work in local Jupyter Notebook.

---

## 🛠️ What The Tool Does

| Step | What Happens |
|------|-------------|
| Step 1 | Installs and imports all libraries |
| Step 2 | Upload your CSV file from your computer |
| Step 3 | Full dataset overview — shape, columns, data types, missing values |
| Step 4 | Detect and rename messy column names |
| Step 5 | Detect and fix wrong data types |
| Step 6A | Handle missing values in numeric columns — 10 options |
| Step 6B | Handle missing values in categorical columns — 7 options |
| Step 7 | Detect and remove duplicate rows — 5 options |
| Step 8 | Detect outliers using IQR and Z-Score with box plots |
| Step 9 | GroupBy analysis with charts for numeric and categorical columns |
| Step 10 | Correlation matrix — NumPy + Pandas + heatmap visualization |
| Step 11 | Download your cleaned CSV file |

---

## 🧠 Cleaning Options

### Missing Values — Numeric
1. Fill with Zero
2. Fill with Mean
3. Fill with Median
4. Fill with a Custom Number
5. Forward Fill
6. Backward Fill
7. Interpolate
8. Drop rows with missing values in specific columns
9. Drop rows where all values are missing
10. Drop the entire column

### Missing Values — Categorical
1. Fill with Mode (most frequent value)
2. Fill with Custom Text
3. Forward Fill
4. Backward Fill
5. Replace a specific value with another
6. Drop rows with missing values
7. Drop the entire column

### Duplicates
1. Keep First occurrence
2. Keep Last occurrence
3. Remove ALL duplicates including the original
4. Remove based on specific columns
5. Skip

### Outliers
1. Remove outlier rows
2. Replace with Median
3. Cap to boundary value
4. Skip

---

## 🔒 Validation & Error Handling

Every input is validated. The tool will never crash silently:
- Wrong column name → error, run cell again
- Number entered where text is expected → error, run cell again
- Text entered where number is expected → error, run cell again
- Empty value entered → error, run cell again
- Invalid menu choice → error, run cell again
- Final output only shows if everything completed successfully

---

## 🧰 Libraries Used

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from scipy import stats
```

---

## 🚀 How To Use

1. Download `CSV_Auto_Cleaner.ipynb`
2. Open [Google Colab](https://colab.research.google.com/)
3. Upload the `CSV_Auto_Cleaner.ipynb` file
4. **⚠️ Read each cell carefully before running it**. Some cells reset or overwrite data. Do not just run everything top to bottom without reading first.
7. Run Step 1 to load all libraries
8. Run Step 2 and upload your CSV file
9. Follow the prompts and type your choices
10. At Step 11 your cleaned file downloads automatically

---

## 💡 What I Learned Building This

- How to handle all types of missing data in numeric and categorical columns
- How IQR and Z-Score detect outliers differently and when each is better
- How GroupBy works for both numeric aggregation and categorical analysis
- How correlation works — the difference between NumPy and Pandas
- How to write input validation and error handling in Python
- Why `display()` causes input bugs in Google Colab and how to fix it

---

## 👩🏾‍💻 Built By

**Benedicta Bondzie (The Tech Diva)**

Solo AI/ML learner. 

Building in public.

---

## 🌍 Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/benedicta-bondzie-the-tech-diva/)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://whatsapp.com/channel/0029VbBL8H8Elagyfxqfxg2I)
[![TikTok](https://img.shields.io/badge/TikTok-000000?style=for-the-badge&logo=tiktok&logoColor=white)](https://www.tiktok.com/@techdiva01)
[![X](https://img.shields.io/badge/X-1DA1F2?style=for-the-badge&logo=x&logoColor=white)](https://x.com/DivaInTech)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/techdiva01)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/@techdivachronicles)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/qr/R4E5YUQKTWDFG1)
[![Substack](https://img.shields.io/badge/Substack-FF6719?style=for-the-badge&logo=substack&logoColor=white)](https://substack.com/@thetechdiva?utm_source=share&utm_medium=android&r=64lok9)

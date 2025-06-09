# Aerofit Treadmill EDA Case Study

This project performs a detailed exploratory data analysis (EDA) on Aerofit treadmill sales and usage data to extract actionable business insights.

#Objective

- Understand customer purchasing behavior
- Identify top-selling treadmill models and regional demand
- Analyze price distribution and product usage
- Recommend strategies for product targeting and marketing

#Dataset

The dataset includes details such as:
- Treadmill model
- Price
- Customer region
- Usage hours
- Purchase trends

> **Note:** Dataset used is `Aerofit.csv`.

## Getting the Data

The original dataset can be downloaded from Kaggle (search for **"Aerofit Treadmill Case Study"**).
Download `Aerofit.csv` and place it in this project directory. If you only want
to experiment with the notebook, you can generate a small sample dataset using
Python:

```python
import pandas as pd
import numpy as np

sample = pd.DataFrame({
    "Product": np.random.choice(["AF204", "AF210", "AF214"], 10),
    "Age": np.random.randint(20, 60, 10),
    "Gender": np.random.choice(["M", "F"], 10),
    "Region": np.random.choice(["East", "West", "North", "South"], 10),
    "Usage": np.random.randint(1, 8, 10),
    "Income": np.random.randint(30000, 90000, 10)
})
sample.to_csv("Aerofit.csv", index=False)
```


#Key Insights

- High-end models priced above \$2000 are less popular in rural regions.
- Model `AF204` had the highest sales across urban metro areas.
- Southern and Western regions show higher average usage per customer.

#Visuals Included

- Price distribution histogram
- Top models bar chart
- Regional demand analysis
- Missing value heatmap
- Correlation matrix (if applicable)

#Tools Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Jupyter Notebook

# Installation

To install the required Python packages, run:

```bash
pip install -r requirements.txt
```

#Business Recommendations

- Focus marketing on top 3 performing regions
- Introduce mid-tier models in underperforming zones
- Offer bundle discounts for older low-selling models

---
## License

This project is licensed under the MIT License - see [LICENSE](LICENSE) for details.


> 👤 By [Sarath Chandra](https://github.com/Sarathchandrrra)

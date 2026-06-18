# Titanic Dataset EDA

This project does basic data cleaning and exploratory data analysis (EDA) on the Titanic dataset.

## Dataset

- Titanic Passenger Data from Seaborn
- 891 passengers, 15 columns
- Contains passenger class, age, gender, survival status, and ticket information

## Technologies

- Python 3.x
- Pandas
- Matplotlib
- Seaborn

## Data Cleaning

1. Loaded the dataset and checked structure
2. Found missing values:
   - Age: 177 missing
   - Embarked: 2 missing
   - Deck: 688 missing (77%)
3. Handled missing values:
   - Age: filled with median (~28 years)
   - Embarked: filled with mode (most common port)
   - Deck: dropped the column (too many missing)
4. Removed duplicate rows
5. Verified no remaining missing values

## Visualizations

1. Survival Count - bar chart
2. Gender Distribution - count plot
3. Age Distribution - histogram
4. Passenger Class Distribution - count plot
5. Survival by Gender - grouped bar chart
6. Correlation Heatmap

## Findings

1. Gender: Females had higher survival rates (~74%) compared to males (~19%)
2. Class: Passenger class affected survival:
   - 1st Class: ~63% survival rate
   - 2nd Class: ~47% survival rate
   - 3rd Class: ~24% survival rate
3. Age: Mean age was ~29.7 years, range from 0.4 to 80 years

## Project Structure

```
harzio-task1/
├── Titanic_Data_Cleaning_Visualization.ipynb
├── data/
│   └── titanic.csv
├── requirements.txt
└── README.md
```

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

2. Open the notebook in Jupyter Notebook or JupyterLab

3. Run all cells

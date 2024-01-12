# Pokemon Data Analysis

## Data Source
The dataset used for this project is sourced from Kaggle and is available [here](https://www.kaggle.com/datasets/abcsds/pokemon).

## Introduction
This project involves the analysis of a Pokemon dataset using Python and various data analysis libraries such as Pandas, Matplotlib, and Seaborn. The dataset contains information about 800 Pokemon, including their types, stats, and other attributes.

## Data Exploration
The initial exploration of the dataset involves loading it into a Pandas DataFrame and checking basic information.

```python
import pandas as pd

# Load dataset
df = pd.read_csv('Pokemon.csv')

# Display basic information
df.info()

# Display descriptive statistics
df.describe()
```

## Data Visualization
The project includes visualizations to better understand the distribution of Pokemon types, totals, and legendary Pokemon.

## Pokemon Types Distribution
Pie chart showing the distribution of Pokemon types:
```python
df['Type 1'].value_counts().plot(kind='pie', autopct='%1.1f%%', cmap='tab20c', figsize=(10, 8))
```

## Pokemon Totals Distribution
Histogram and box plot for the distribution of Pokemon totals:

```python
df['Total'].plot(kind='hist', figsize=(10, 8))
df['Total'].plot(kind='box', vert=False, figsize=(10, 5))
```

## Legendary Pokemon Distribution
Pie chart showing the distribution of legendary Pokemon:
```python
df['Legendary'].value_counts().plot(kind='pie', autopct='%1.1f%%', cmap='Set3', figsize=(10, 8))
```
## Basic Filtering
Several basic filtering operations are performed, including finding powerful Pokemon based on attack values and selecting Pokemon with specific attributes.

## Advanced Selection
More advanced selection queries are used to filter Pokemon based on specific criteria, such as type, generation, and stats.

## Conclusion
The project concludes with a summary of the analysis, showcasing the most powerful and unique Pokemon based on various criteria.

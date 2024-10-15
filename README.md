# IPL Auction 2023 Data Analysis

This project performs exploratory data analysis (EDA) on the IPL Auction 2023 dataset. The dataset contains information about players, their styles, nationalities, base and final prices, and auction status. The analysis focuses on gaining insights into the auction process, player categories, and pricing trends.

## Dataset Overview

The dataset contains the following columns:
- **name**: Name of the player.
- **player style**: Player's role (Bowler, Batter, Allrounder, WK-Batter).
- **nationality**: Nationality of the player.
- **base price (in lacs)**: The base price set for the player during the auction.
- **final price (in lacs)**: The final price at which the player was sold (if applicable).
- **franchise**: The franchise that bought the player.
- **status**: Player's auction status (SOLD, UNSOLD, RETAINED).

## Key Operations

1. **Data Preprocessing**:
   - Handled missing values by filling `NaN` in `base price` and `final price` with 0.
   - Converted data types of `base price` and `final price` to integers.
   - Applied `map()` and `replace()` functions to update the `status` column values.

2. **Descriptive Statistics**:
   - Used `describe()` to generate summary statistics for both numerical and categorical columns.
   - Computed the mean, maximum, and unique values for base and final prices.

3. **Grouping and Aggregation**:
   - Grouped data by `status` and calculated various statistics like mean, standard deviation, and min-max values using `agg()`.

4. **Visualization**:
   - Created count plots using `seaborn` to visualize the distribution of players by nationality and auction status.
   - Analyzed how many players were sold at their base price using cross-tabulation and visualized with count plots.

## Key Insights

- The dataset shows trends of player sales based on base price and nationality.
- The relative frequency of player styles and nationality in the auction is examined.
- Visualization helps understand which nationalities had the most players sold, retained, or unsold.

## Dependencies

- Python 3.x
- Libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`

## How to Run

1. Install the necessary dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn

## Conclusion


This `README.md` gives a concise yet informative overview of your IPL Auction 2023 project and outlines the main steps of your EDA.

  

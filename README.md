# Analyze-Death-Age-Difference-of-Right-Handers-with-Left-Handers
I will provide the README content in Markdown format.

-----

# Where are the Old Left-Handed People? 🖐️👴👵

## Unraveling the Mystery of Handedness and Longevity

This project explores a fascinating demographic puzzle: the apparent scarcity of older left-handed individuals. While a 1986 National Geographic survey observed a significant decline in left-handedness with increasing age (from \~13% for under 40s to \~5% for 80-year-olds), this project aims to demonstrate that this difference in average age at death can be explained purely by the historical changes in the social acceptability and reporting of left-handedness over time, rather than a biological predisposition to earlier death for left-handers.

Using statistical analysis, particularly **Bayesian statistics**, we will reproduce this age difference and show that the "missing" old left-handers are a consequence of birth year effects, not premature mortality.

## 🚀 Project Goals

  * **Visualize Historical Handedness Trends**: Plot the rates of left-handedness as a function of age and, crucially, as a function of birth year to illustrate the changing prevalence over time.
  * **Apply Bayes' Theorem**: Utilize conditional probability to calculate the probability of dying at a certain age given one's handedness: $P(\\text{Age at Death} | \\text{Handedness})$.
  * **Analyze Death Distribution Data**: Incorporate real-world death distribution data (from the US in 1999) to understand the general probability of dying at any given age.
  * **Determine Overall Handedness Probabilities**: Calculate the overall probability of being left-handed within the deceased population.
  * **Compare Age at Death Distributions**: Plot and compare the probability distributions of age at death for both left-handed and right-handed individuals.
  * **Calculate Average Age at Death**: Quantify the average age at death for each handedness group and determine the difference.
  * **Explore Modern Implications**: Re-evaluate the age gap if the study were conducted today (e.g., in 2018) to observe how changing historical trends impact the results.

## 📊 Data Sources

This analysis uses two key datasets:

1.  **Left-handedness Rates**: Digitized from a figure in a [1992 paper by Gilbert and Wysocki](https://www.ncbi.nlm.nih.gov/pubmed/1528408) based on the 1986 National Geographic survey. This dataset provides age-specific rates of left-handedness for males and females.

      * `lh_data.csv`: Accessible via raw Gist link.

2.  **Death Distribution Data**: For the United States in the year 1999, sourced from the CDC. This data provides the number of deaths per age group, allowing us to estimate the probability of dying at a particular age.

      * [CDC Source Website](https://www.cdc.gov/nchs/nvss/mortality_tables.htm)
      * `cdc_vs00199_table310.tsv`: Accessible via raw Gist link.

## 💻 Technologies Used

  * `Python`
  * `pandas` for data manipulation and analysis
  * `numpy` for numerical operations
  * `matplotlib` for data visualization

## ✨ Key Insights & Findings (Spoiler Alert\!)

Our analysis demonstrates that the observed age gap between left-handed and right-handed individuals at death can be largely explained by the generational shift in left-handedness prevalence. Historically, societal pressures led to a lower reported rate of left-handedness among older generations. When observing a sample of recently deceased individuals, this means there will naturally be more older right-handers, creating an *apparent* age difference.

The project highlights the importance of considering historical context and demographic changes when interpreting statistical observations. The "early death" claim for left-handers is likely a statistical artifact rather than a biological reality.

## 🏃 How to Run the Project

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    cd your-repository-name
    ```
2.  **Create a Virtual Environment (Recommended)**:
    ```bash
    python -m venv venv
    # On Windows
    .\venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```
3.  **Install Dependencies**:
    ```bash
    pip install pandas numpy matplotlib
    ```
4.  **Open and Run the Jupyter Notebook**:
    ```bash
    jupyter notebook notebook.ipynb
    ```
    Follow the instructions within the `notebook.ipynb` file to execute the code cells sequentially and observe the analysis unfold.

## 🤝 Contributing

Contributions are welcome\! If you have suggestions for improvements, new features, or find any issues, please open an issue or submit a pull request.

## 📄 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE).

-----

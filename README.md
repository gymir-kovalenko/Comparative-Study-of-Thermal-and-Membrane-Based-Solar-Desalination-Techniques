
# Comparative Study of Thermal and Membrane-Based Solar Desalination Techniques

This project presents a comprehensive analysis of two primary solar desalination techniques — **Thermal-based** and **Membrane-based** — using a structured Python codebase in Jupyter Notebook format. The objective is to evaluate, compare, and visualize the performance of these methods based on a custom dataset.

---

## 📁 Project Structure

```text
.
├── 01_Data_Exploration.ipynb              # Dataset loading and initial analysis
├── 02_Statistical_Comparison.ipynb        # Statistical t-tests between techniques
├── 03_ML_Model_Comparison.ipynb           # Machine Learning classifier to distinguish techniques
├── 04_Conclusion_and_Visualization.ipynb  # Final graphs and conclusion
├── desalination_system_data.csv           # Dataset for analysis
└── README.md                              # Project documentation
```

---

## 📄 Dataset Description: `desalination_system_data.csv`

This dataset contains simulated or real-world data from solar desalination systems, with the following columns:

| Column Name        | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `solar_irradiance` | Solar energy incident on the system (W/m²)                                  |
| `battery_charge`   | Battery status or energy storage level (%)                                  |
| `energy_use`       | Energy consumed by the system (kWh)                                         |
| `feedwater_salinity` | Salinity of the incoming water (ppm)                                     |
| `pressure`         | System pressure (bar)                                                       |
| `freshwater_output`| Freshwater produced by the system (liters/hour)                             |
| `system_efficiency`| Efficiency of the system calculated based on energy use and output (%)      |
| `technique`        | Type of desalination system (`thermal` or `membrane`)                       |

---

## 🧪 1. Data Exploration

- Load the dataset using `pandas`
- Perform `info()`, `describe()`, and null-value checks
- Generate distribution plots for key variables like `system_efficiency` and `freshwater_output`
- Visualize how efficiency differs between thermal and membrane techniques using `seaborn`

---

## 📊 2. Statistical Comparison

- Filter data based on `technique`
- Perform independent **t-test** to compare mean efficiencies
- Determine if the performance difference is **statistically significant**

---

## 🤖 3. ML Model Comparison

- Convert `technique` to binary labels (`thermal`=0, `membrane`=1)
- Split data into training and testing sets
- Train a **Random Forest Classifier** to see if system features can predict the technique
- Evaluate model using **classification report** (precision, recall, F1-score)

---

## 📈 4. Final Visualization & Conclusion

- Visualize average system efficiencies using bar plots
- Interpret which system is better based on efficiency and output
- Provide insights into use-case scenarios where each technique is preferable

---

## ✅ Key Findings

- **Membrane-based systems** often show higher average efficiency, especially under stable energy supply
- **Thermal systems** may be more resilient in fluctuating conditions with high solar input
- Machine learning models can distinguish between systems based on operational metrics

---

## 📌 Future Improvements

- Include cost analysis per liter of freshwater output
- Integrate time-series performance under varying environmental conditions
- Expand ML model to include more algorithms (e.g., SVM, Gradient Boosting)
- Test on real-world datasets from desalination plants

---

## 📚 References

- Research articles on solar desalination techniques
- Textbooks on water treatment and renewable energy systems
- Scikit-learn documentation for model training
- Please find Dataset for operations : https://drive.google.com/file/d/1QHx9aTSheQ0Sxth-DVuM0ogmaYLSW-CB/view?usp=sharing

---

## 🚀 How to Run

1. Open the notebooks in [JupyterLab](https://jupyter.org/) or [Google Colab](https://colab.research.google.com/)
2. Ensure `desalination_system_data.csv` is in the same directory
3. Execute the notebooks in order: `01_...` ➝ `04_...`

---

## 🧑‍💻 Author

This project was created as part of a B.Tech final year thesis for studying sustainable water technologies using machine learning and statistical analysis.


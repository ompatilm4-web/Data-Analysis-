# 📊 Python Data Science Toolkit

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.26+-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13+-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

<br/>

> **A structured, hands-on repository for mastering Python's core Data Science libraries — from fundamentals to real-world data analysis.**

<br/>

[![Stars](https://img.shields.io/github/stars/yourusername/yourrepo?style=social)](https://github.com/yourusername/yourrepo)
[![Forks](https://img.shields.io/github/forks/yourusername/yourrepo?style=social)](https://github.com/yourusername/yourrepo)

</div>

---

## 📁 Repository Structure

```
📦 Python-Data-Science-Toolkit
 ┣ 📓 Numpy.ipynb          → NumPy arrays, broadcasting, linear algebra
 ┣ 📓 Pandas.ipynb         → DataFrames, cleaning, merging, aggregation
 ┣ 📓 Matplotlib.ipynb     → Static plots, customization, subplots
 ┣ 📓 Seaborn.ipynb        → Statistical visualizations, heatmaps, distributions
 ┣ 📄 Practice.md          → 40 hard practice questions (NumPy + Pandas)
 ┣ 📊 Sale_data.csv        → Real-world sales dataset for practice
 ┣ 📊 data.csv             → Student records dataset
 ┗ 📊 output.csv           → Generated output from Pandas operations
```

---

## 🧠 What's Inside

### 🔢 NumPy — `Numpy.ipynb`

> The foundation of numerical computing in Python.

- ✅ Creating and reshaping N-dimensional arrays
- ✅ Broadcasting rules and vectorized operations
- ✅ Advanced indexing and boolean masking
- ✅ Linear algebra — eigenvalues, matrix multiplication, dot products
- ✅ Statistical operations — mean, std, covariance
- ✅ Practical applications: normalization, checkerboard patterns, PCA

**Key Concepts Covered:**
| Concept | Description |
|---|---|
| `np.array` | Creating 1D, 2D, nD arrays |
| `np.reshape` | Changing array dimensions |
| Broadcasting | Operating on arrays of different shapes |
| `np.linalg` | Eigenvalues, inverse, determinant |
| Indexing | Fancy, boolean, slice-based |

---

### 🐼 Pandas — `Pandas.ipynb`

> The go-to library for data manipulation and analysis.

- ✅ Creating `Series` and `DataFrame` objects from lists, dicts, and CSV files
- ✅ Exploratory Data Analysis (EDA) — `head()`, `tail()`, `describe()`, `info()`
- ✅ Data selection — `loc`, `iloc`, column filtering, conditional filtering
- ✅ Handling missing values — `isnull()`, `fillna()`, `dropna()`
- ✅ Sorting, ranking, and applying lambda functions
- ✅ GroupBy operations with single and multi-column aggregation
- ✅ DataFrame merging — inner, outer, left, right joins
- ✅ Reading from CSV and JSON data sources
- ✅ Exporting results to CSV with `to_csv()`

**Key Operations Demonstrated:**
```python
# GroupBy + Aggregation
Sales_Data.groupby(['Product', 'Category'])['Quantity'].agg(['sum', 'mean', 'count'])

# Merge DataFrames
pd.merge(df1, df2, on="keys", how="inner")

# Apply custom logic
df["Salary"].apply(lambda x: x * 2)
```

---

### 📈 Matplotlib — `Matplotlib.ipynb`

> Python's primary plotting library for static, publication-quality figures.

- ✅ Line plots, bar charts, scatter plots, histograms, pie charts
- ✅ Customizing titles, axis labels, legends, and colors
- ✅ Creating subplots with `plt.subplot()` and `fig, ax` syntax
- ✅ Saving figures to files
- ✅ Annotating and styling charts for presentations

---

### 🎨 Seaborn — `Seaborn.ipynb`

> Statistical data visualization built on top of Matplotlib.

- ✅ Distribution plots — `histplot`, `kdeplot`, `boxplot`, `violinplot`
- ✅ Relationship plots — `scatterplot`, `lineplot`, `pairplot`
- ✅ Categorical plots — `barplot`, `stripplot`, `swarmplot`
- ✅ Heatmaps for correlation matrices
- ✅ FacetGrid for multi-variable comparison
- ✅ Built-in themes and color palettes

---

### 🏋️ Practice — `Practice.md`

> **40 carefully crafted, interview-level problems** to sharpen your skills.

#### 🔹 NumPy (20 Questions)
| Category | Topics |
|---|---|
| Array Logic | Border replacement, row swapping, checkerboard |
| Broadcasting | Row-wise addition, column subtraction, matrix creation |
| Linear Algebra | Eigenvalues, cosine similarity, PCA, covariance |

#### 📊 Pandas (20 Questions)
| Category | Topics |
|---|---|
| Data Cleaning | IQR outliers, datetime parsing, conditional replacement |
| GroupBy | Top-N per group, % contribution, department ranking |
| Merging | Inner/left/right joins, anti-joins, 3-dataset merge |
| Advanced | Pivot tables, rolling averages, memory optimization |

---

## 🗃️ Datasets

### 📊 `Sale_data.csv`
- Contains product sales records with fields: `Product`, `Category`, `Quantity`, etc.
- Used for GroupBy, aggregation, and merging exercises in Pandas notebooks.

### 📊 `data.csv`
- Contains student records with `ID`, `Name`, `Marks` fields.
- Used for data manipulation, column creation, and group operations.

### 📊 `output.csv`
- Auto-generated by `Pandas.ipynb` from the `to_csv()` demonstration.
- Contains `Name`, `City`, `Salary`, `Bonus` columns used in GroupBy examples.

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.10+ installed. Then install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### Run the Notebooks

```bash
# Clone the repository
git clone https://github.com/yourusername/yourrepo.git
cd yourrepo

# Launch Jupyter Notebook
jupyter notebook
```

Open any `.ipynb` file from the Jupyter interface in your browser.

---

## 💡 Learning Path

Follow this sequence for the best learning experience:

```
NumPy  →  Pandas  →  Matplotlib  →  Seaborn  →  Practice (40 Qs)
 🔢          🐼           📈             🎨              🏋️
```

> 💡 **Tip:** Attempt at least 5 practice questions daily. Avoid loops in NumPy — always prefer vectorization.

---

## 🎯 Skills You'll Build

After completing this repository, you will be able to:

- 🔢 **Manipulate** multi-dimensional arrays efficiently using NumPy
- 🐼 **Clean, transform, and analyze** real-world datasets using Pandas
- 📈 **Visualize** data insights clearly using Matplotlib and Seaborn
- 🧩 **Solve** interview-level data science problems independently
- 🤖 **Prepare** your foundations for Machine Learning workflows

---

## 📚 Resources

- 📘 [NumPy Official Docs](https://numpy.org/doc/)
- 🐼 [Pandas Official Docs](https://pandas.pydata.org/docs/)
- 📊 [Matplotlib Official Docs](https://matplotlib.org/stable/index.html)
- 🎨 [Seaborn Official Docs](https://seaborn.pydata.org/)
- 📓 [Jupyter Notebook Docs](https://jupyter.org/documentation)

---

## 🤝 Contributing

Contributions, suggestions, and new practice questions are welcome!

1. Fork the repository
2. Create a new branch (`git checkout -b feature/add-question`)
3. Commit your changes (`git commit -m 'Add new practice question'`)
4. Push to the branch (`git push origin feature/add-question`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">

**Made with ❤️ for Data Science learners**

⭐ Star this repo if it helped you learn something new!

</div>

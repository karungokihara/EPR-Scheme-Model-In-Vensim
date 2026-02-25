# UK Extended Producer Responsibility (EPR) Policy Model

**A System Dynamics simulation and data extraction tool for evaluating the UK's EPR scheme.**

## 📌 Project Overview

This repository contains a Vensim-based simulation model designed to evaluate the impacts of the **Extended Producer Responsibility (EPR)** policy in the UK.

The project integrates **System Dynamics** with **Python** via the `PySD` library. This allows the model logic (developed in Vensim) to be executed within a Python environment for high-speed data extraction, automated sensitivity analysis, and formatted CSV exporting.

## 📂 Project Structure

* **`Policy1and2_V11.mdl`**: The source Vensim model containing the stocks, flows, and feedback loops of the EPR policy.
* **`Main.py`**: The "Engine." This script loads the `.mdl` file, runs the simulation, and processes the output.
* **`requirements.txt`**: List of Python libraries needed (PySD, Pandas, etc.).
* **Datasets (Baselines)**:
* `projection_detailed_total_vensim_input.csv`: Primary input for volume projections.
* `rates.csv`: Economic and recovery rate data.
* `transferrates.csv`: Logistics and transfer efficiency data.



## 🚀 Getting Started

### 1. Prerequisites

* **Vensim:** Required to edit the `.mdl` file.
* **Python 3.8+**: Required to run the extraction scripts.

### 2. Installation

Open your terminal and run:

```bash
git clone https://github.com/karungokihara/EPR-Scheme-Model-In-Vensim.git
cd EPR-Scheme-Model-In-Vensim
pip install -r requirements.txt

```

## 📊 How to Run

### Option A: Manual Vensim Run

1. Open `Policy1and2_V11.mdl` in Vensim.
2. Ensure the 3 CSV files are in the same folder as the model.
3. Run the simulation (`Ctrl+R`) to view graphs and tables within Vensim.

### Option B: Automated Python Extraction (Recommended)

This method uses `PySD` to translate the Vensim model into Python code on the fly.

1. Run the main script:
```bash
python Main.py

```


2. **What happens?** * The script initializes the model logic.
* It pulls data from the baseline CSVs.
* It exports the results into a formatted CSV file for policy reporting.



---

## ☕ Support

If you find this research or model helpful, feel free to support my work:

## 📩 Contact

For inquiries, policy collaborations, or technical feedback:
**Email:** [karungokihara@gmail.com](mailto:karungokihara@gmail.com)

---

## 📝 License

This project is for research and policy evaluation purposes. (MIT License)
---
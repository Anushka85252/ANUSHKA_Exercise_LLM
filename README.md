# LLM-Based Code Generation for Energy Consumption Analysis

This project demonstrates how large language models (LLMs) can be used to translate natural language queries into executable Python code for analyzing household power consumption data. The focus is on using LLMs to perform time-series data analysis with `pandas` on a real-world dataset.

---

## 👤 Author

**Anushka Sanjay Shelke**

---

## 💻 LLM Used

This project used the **Groq Cloud Playground** to generate Python code from natural language prompts.

- **Model:** `meta-llama/llama-4-scout-17b-16e-instruct`
- **Temperature:** 1.0  
- **Top-p:** 1.0  
- **Max tokens:** 1024  

---

## 📊 Dataset

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)
- **File used:** `household_power_consumption.csv`

### Preprocessing Steps

The original `.txt` dataset was converted to CSV and preprocessed using pandas:
- Combined `Date` and `Time` into a datetime index
- Parsed missing values marked as `'?'`
- Converted `Global_active_power` to float
- Set `datetime` as the index for time-series operations

---

## ✅ Tasks Completed

This notebook contains the following analysis tasks, each handled using prompts processed by the LLaMA 4 model:

1. **Calculate average active power consumption in March 2007?**
2. **Find the hour with highest power usage on December 25, 2006?**
3. **Compare weekday vs. weekend energy consumption**
4. **Identify days with energy usage over 5 kWh**
5. **Visualize power usage for the first week of January 2007**
6. **Calculate average voltage per day for the first week of February 2007**
7. **Find correlation between `Global_active_power` and sub-metering values?**

---

## 📁 Project Structure

## ⚙️ Getting Started

1. **Clone this repository:**

   ```bash
   git clone https://github.com/Anushka85252/ANUSHKA_Exercise_LLM.git
   cd ANUSHKA_Exercise_LLM

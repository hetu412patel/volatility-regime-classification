# volatility-regime-classification
An end-to-end analytics pipeline for classifying stock market volatility regimes using FTSE 100 data (1999–2025). Combines statistical analysis and a Random Forest model (AUC: 0.965, F1: 0.929) to identify crisis vs. non-crisis periods, with results visualised through an interactive Power BI dashboard for investor decision support.

## Tools & Technologies
- Python
- Orange (Data Mining & Machine Learning)
- Power BI (Data Visualization & Dashboarding)
  
## Setup & Execution Guide

Follow these steps to run the project locally:

**1. Clone the Repository**
  - git clone <your-repo-url>
    Or download the ZIP and extract it into your preferred folder.

**2. Open in VS Code**
  - Launch the project folder in Visual Studio Code.
  - Ensure the Jupyter Notebook extension is installed.
    
**3. Configure Python Environment**
  - Select or create a Python environment (recommended: virtual environment).
  - Make sure it is set as the active interpreter in VS Code.
    
**4. Install Required Dependency**
  - pip install yfinance
    
**5. Run Jupyter Notebooks**
  - Execute both notebook files in sequence:
      Notebook 1 → Generates intermediate output (Data collection & EDA)
      Notebook 2 → Uses output from Notebook 1 as input (Volatility behaviour)
    
**6. Generate Feature Matrix**
  - After running Notebook 2, a feature matrix CSV file will be generated.
    
**7. Install Orange**
  - Download and install Orange from its official website.
    
**8. Load Data in Orange**
  - Open Orange Canvas.
  - Use the File widget to import the generated feature matrix CSV file.
  - Configure the workflow by connecting the required widgets (as per the provided Orange workflow      file), including data preprocessing, model (e.g., Random       Forest) and evaluation components.
  - Run the workflow to classify the data into volatility regimes (crisis vs. non-crisis).
  - Analyze model performance and save the classified output using the appropriate widgets (e.g Save Data).

## Orange Workflow
<img width="940" height="592" alt="image" src="https://github.com/user-attachments/assets/4ada3180-f5c3-4773-b8f0-def2c61a8b15" />

# 📊 Power BI Dashboard (with Python Integration)

## 🔍 Overview
The final stage of this project is an **interactive Power BI dashboard** that transforms complex financial analytics into intuitive decision-support insights.

It combines:
- Volatility analysis  
- Machine learning outputs  
- Interactive visualisation  
- Investment decision support  
---

## 🧰 Tools Used
- Power BI Desktop  
- Python  

### Python Libraries
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
---

## ⚠️ Setup (IMPORTANT)

### Install Python Libraries
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
---

### Configure Python in Power BI
1. Open Power BI Desktop  
2. Go to: File → Options → Python scripting  
3. Select your Python path  
---

## 📁 Power BI File
`Participant-04 Power BI File.pbix`
> GitHub cannot preview `.pbix` files — download and open in Power BI Desktop  
---

## 📈 Dashboard Pages
---

### 1. Volatility Overview Dashboard
<img width="940" height="522" alt="Volatility Overview Dashboard" src="https://github.com/user-attachments/assets/e2b1e928-63f1-4f74-bf9e-512dc11bd0eb" />

**Features:**
- Time-series volatility (2000–2025)  
- Crisis vs Non-Crisis classification  
- Adaptive threshold  
- Interactive filters  
---

### 2. Indicator Importance Panel
<img width="940" height="546" alt="Indicator Importance Dashboard" src="https://github.com/user-attachments/assets/0c87d0a5-580f-489c-a3c6-9e1b0d0c44c7" />

**Features:**
- Indicator comparison  
- Distribution analysis  
- Feature importance  
- Statistical differences  
---

### 3. Predictive Modelling Dashboard
<img width="940" height="532" alt="Predictive Modelling Dashboard" src="https://github.com/user-attachments/assets/502ffd2a-da01-4e6b-a2ae-2ee033296cf2" />

**Features:**
- Random Forest results  
- Confusion matrix  
- Accuracy: 92.8%  
- Probability distribution  
- Clustering  
---

### 4. Investment Decision Support Dashboard
<img width="940" height="530" alt="Investment Decision Dashboard" src="https://github.com/user-attachments/assets/90e16d4c-4833-4770-8fdb-f908d5518b1c" />

**Features:**
- What-if parameters  
- Investment score  
- Decision output:
  - Invest  
  - Caution  
  - Avoid  
---

## ▶️ How to Use

1. Open `.pbix` file  
2. Navigate pages  
3. Use filters  
4. Adjust sliders for simulation  
---

## 🧠 Key Contribution

- Volatility regime classification using ML  
- Integration of Python + Power BI  
- Interactive decision support system  
- Designed for non-technical users  
---

## 📌 Notes

- Python must be installed  
- Ensure libraries are installed  
- Check Python path in Power BI if visuals fail  
- Use latest Power BI Desktop  
---

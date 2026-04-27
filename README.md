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
  - 
**3. Configure Python Environment**
  - Select or create a Python environment (recommended: virtual environment).
  - Make sure it is set as the active interpreter in VS Code.
  - 
**4. Install Required Dependency**
  - pip install yfinance
  - 
**5. Run Jupyter Notebooks**
  - Execute both notebook files in sequence:
      Notebook 1 → Generates intermediate output (Data collection & EDA)
      Notebook 2 → Uses output from Notebook 1 as input (Volatility behaviour)
    
**6. Generate Feature Matrix**
  - After running Notebook 2, a feature matrix CSV file will be generated.
  - 
**7. Install Orange**
  - Download and install Orange from its official website.
  - 
**8. Load Data in Orange**
  - Open Orange Canvas.
  - Use the File widget to import the generated feature matrix CSV file.
  - Configure the workflow by connecting the required widgets (as per the provided Orange workflow      file), including data preprocessing, model (e.g., Random Forest),        and evaluation components.
  - Run the workflow to classify the data into volatility regimes (crisis vs. non-crisis).
  - Analyze model performance and save the classified output using the appropriate widgets (e.g Save Data).

## Orange Workflow
<img width="940" height="592" alt="image" src="https://github.com/user-attachments/assets/4ada3180-f5c3-4773-b8f0-def2c61a8b15" />


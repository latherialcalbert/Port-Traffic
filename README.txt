US Port Traffic Data Analysis and Prediction
This repository contains a data science project that analyzes historic US port traffic data and predicts future trends using machine learning techniques. The project focuses on import/export activities across various US ports, utilizing data collected from specific sources, including aappa and scscpa port websites.

Project Overview
The workflow for this project involves:
    1 Data Collection:
        ◦ Historic US port traffic data sourced from official websites, including:
            ▪ aappa (American Association of Port Authorities).
            ▪ scscpa (South Carolina State Ports Authority).
    1 Data Cleaning and Preparation:
        ◦ Utilized the DataPrepPort_aappa.ipynb notebook to preprocess datasets.
        ◦ Standardized and formatted the data for further analysis.
        ◦ Addressed outliers and inconsistencies using custom scripts.
    1 Data Combination:
        ◦ Used csv_combiner.ipynb to merge datasets from different sources into a single consolidated dataset for model building.
    1 Model Training:
        ◦ Built predictive models using polynomial regression to analyze traffic trends.
        ◦ Evaluated model performance with metrics such as R², MSE, RMSE, and MAE.
    1 Visualization and Prediction:
        ◦ Generated visualizations to showcase historic trends and future projections.
        ◦ Focused on traffic data trends from 1972 to 2024.

Repository Structure
US-port-traffic-analysis/
|—— clean_files_sorted/
|    Sorted files by region
|—— combined_csv_file_for_model/
|    Final consolidated dataset used for training and testing.
|—— historic_us_files_separated/
|    Original datasets categorized by year.
|—— scscpa_csv/
|    Traffic data specifically from the South Carolina State Ports Authority.
    |—— DataPrepPort_Scscpa.ipynb
	Scscpa port file cleaning and prep for final dataset
|—— DataPrepPort_aappa.ipynb
|    Notebook for preprocessing data from aappa sources.
|—— csv_combiner.ipynb
|    Notebook for combining multiple CSV files into a single dataset.
|—— US_port_traffic_models.ipynb
     Notebook for data analysis, model training, and visualization.

Key Features
    • Data Cleaning:
        ◦ Preprocessing tailored to specific sources such as aappa and scscpa websites.
        ◦ Handling missing values, duplicates, and data normalization.
    • Advanced Modeling:
        ◦ Polynomial regression models for trend prediction.
        ◦ Evaluated models on separate training and validation datasets.
    • Comprehensive Visualizations:
        ◦ Historic data trends and theoretical projections.
        ◦ Baseline metrics for comparison with model predictions.

Instructions to Run
    1 Clone the Repository: git clone https://github.com/yourusername/US-port-traffic-analysis.git
    1 cd US-port-traffic-analysis
    1 Install Dependencies:
        ◦ Required libraries: numpy, pandas, matplotlib, scikit-learn.
        ◦ Install via pip: pip install numpy pandas matplotlib scikit-learn
    1 Run the Data Cleaning Notebook:
        ◦ Open DataPrepPort_aappa.ipynb to preprocess aappa datasets.
        ◦ For scscpa datasets, refer to scscpa_csv/ and include files in csv_combiner.ipynb.
    1 Combine CSV Files:
        ◦ Use csv_combiner.ipynb to merge cleaned files into one consolidated dataset.
    1 Train and Test Models:
        ◦ Run US_port_traffic_models.ipynb to analyze trends and generate predictions.

Future Scope
    • Automate data scraping directly from aappa and scscpa websites.
    • Extend modeling to include more advanced techniques such as ensemble models or deep learning.
    • Develop interactive dashboards for real-time trend analysis.

Note:
Original scraped files are not available due to size limitations but examples of the pipeline are demonstrated. PDF's from websites were scraped and converted to csv files and cleaned. This is also not shown due to file size limitations.


License
This project is licensed under the MIT License. See the LICENSE file for details.

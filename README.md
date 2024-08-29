# Developing an Early Prediction Model for Age-Related Hearing Loss Using the Taiwan Biobank
This project aims to develop an early prediction model for age-related hearing loss using data from the Taiwan Biobank. By analyzing physical examination data, lifestyle factors, and SNP locus data, the model seeks to identify individuals at risk of hearing decline in older age, allowing for earlier interventions and better management.

## Data Source
The dataset includes 165 features from questionnaires covering lifestyle habits, family medical history, female physiological conditions, traditional Chinese medicine consultations, and physical examination data. Participants were categorized into two groups based on hearing loss status, with 5,603 individuals having hearing loss and 12,400 with normal hearing.

## Requirements
To run the analysis, you'll need Python 3.8 or above and the following libraries:
```bash
pandas==1.2.4
numpy==1.21.0
scikit-learn==1.4.2
matplotlib==3.3.4
seaborn==0.11.1
imblearn==0.12.3
xgboost==2.0.2
shap==0.46.0
tensorflow==2.17.0
```

## Usage
```bash
notebook/SNP/                # Directory containing SNP feature data and related analysis
notebook/clean_data.ipynb    # Data cleaning
notebook/select_feature_*    # Feature selection
notebook/predict_*           # Model prediction
resource/                    # Details of data source columns
result/                      # Output from data analysis and feature selections
README.md                    # Project overview and instructions
```

To run these notebooks, navigate to the `notebook` directory and open each `.ipynb` file in Jupyter Notebook. You can start Jupyter Notebook by running the following command in your terminal:
```bash
jupyter notebook
```
Once Jupyter Notebook is running, open the notebook files in order and execute the cells step by step to reproduce the analysis.

## Results
The final analysis identified key features for predicting hearing loss, with 10 significant features for males and 20 for females. The prediction model achieved an average F1 score of 0.76 for males and 0.78 for females. Notably, 5 features were common predictors for both genders. Future research will focus on further analyzing SNP data related to hearing loss.

## Collaboration
This project is a collaborative effort with the Institute of Information Engineering at Academia Sinica.

## Contact
For questions or feedback, please contact ss612270623@gmail.com.

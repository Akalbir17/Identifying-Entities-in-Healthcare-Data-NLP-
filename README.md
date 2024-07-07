# Identifying Entities in Healthcare Data using NLP

## Table of Contents
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Methodology](#methodology)
  - [Data Preprocessing](#data-preprocessing)
  - [Concept Identification](#concept-identification)
  - [Feature Engineering](#feature-engineering)
  - [Model Building](#model-building)
  - [Evaluation](#evaluation)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)
- [Conclusion](#conclusion)

## Problem Statement
BeHealthy, a health tech company, aims to connect the medical community with millions of patients across the country through its web platform. The platform allows doctors to list their services, manage patient interactions, and provide online consultations. As a result, BeHealthy generates a vast amount of medical data daily.

The objective of this project is to develop an algorithm that can identify diseases and their respective treatments from the medical data generated on the BeHealthy platform. The data is in the form of unstructured text, such as doctor's notes or therapy reviews, and contains medical terms that may not be easily understood by a non-medical audience.

## Dataset
The dataset consists of medical text data containing information about diseases and their treatments. The data is not explicitly labeled, but the diseases and treatments can be inferred from the context of the text.

## Methodology

### Data Preprocessing
- Perform data cleaning and preprocessing steps to handle missing values, remove special characters, and convert the text to lowercase.
- Tokenize the text data into individual words or tokens.

### Concept Identification
- Identify medical concepts such as diseases, treatments, and body parts using medical knowledge bases or dictionaries like UMLS (Unified Medical Language System).
- Map the identified concepts to their corresponding entity types (e.g., disease, treatment).

### Feature Engineering
- Define features for the Conditional Random Field (CRF) model, such as word embeddings, part-of-speech tags, and entity types.
- Extract features and labels from the preprocessed text data.

### Model Building
- Split the data into training and testing sets.
- Build a CRF model using the extracted features and labels.
- Train the CRF model on the training data.

### Evaluation
- Evaluate the trained CRF model on the testing data using metrics such as precision, recall, and F1-score.
- Fine-tune the model hyperparameters to improve performance.

## Results
- The custom CRF model achieved a training F1-score of 93.12% and a test F1-score of 91.89%.
- The model successfully identified diseases and their corresponding treatments from the medical text data.
- For example, the model predicted that the treatment for "Hereditary Retinoblastoma" is "Radiotherapy".

## Requirements
- Python 3.7+
- pandas
- numpy
- scikit-learn
- nltk
- matplotlib
- seaborn
- jupyter

## Usage
1. Clone the repository: git clone https://github.com/Akalbir17/Identifying-Entities-in-Healthcare.git
  
2. Install the required dependencies: `pip install-r requirements.txt`

3. Place the medical text data in the `data/` directory.

4. Open the Jupyter Notebook `notebooks/Identifying_Entities_in_Healthcare_Data.ipynb`[1] and run the cells to preprocess the data, build the CRF model, and evaluate its performance.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Conclusion
In this project, we successfully developed a custom CRF model to identify diseases and their corresponding treatments from medical text data. The model achieved high performance, with a training F1-score of 93.12% and a test F1-score of 91.89%. By leveraging NLP techniques and domain-specific knowledge, we were able to extract valuable insights from unstructured medical data, which can assist healthcare professionals in making informed decisions and improving patient care.


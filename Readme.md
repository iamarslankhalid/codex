# **Greeklish Classification Project**

## Setup Instructions

### 1. Install Dependencies

- Ensure you have Python 3.x installed, then install the required libraries:

- `pip install -r requirements.txt`

- Alternatively, install dependencies manually:

- `pip install pandas numpy scikit-learn nltk joblib`

### 2. Running the Scripts

#### 2.1. Scraping Data

- python greeklish_scraping.py

- This script scrapes Greeklish and English sentences and saves them to final_dataset.csv.

#### 2.2. Preprocessing the Data

- python preprocess_data.py

- Splits paragraphs into sentences and cleans text, saving results to sentences_dataset.csv.

#### 2.3. Training the Model

- python train_svm.py

- Trains an SVM classifier and saves the model as greeklish_svm_model.pkl.

#### 2.4. Evaluating the Model

- python evaluate_model.py

- Prints accuracy, precision, recall, and F1-score.

### 3. Testing the Classifier

- To classify a new sentence:

- python predict.py "ti kaneis"

- Output:

- Prediction: Greeklish

#### **Notes**

- The model uses TF-IDF with character n-grams.

- The SVM classifier is trained using an RBF kernel.

- All datasets and models are stored in /mnt/data/ for easy access.

- For further details, refer to the Documentation PDF.
# **Greeklish Classification Project**

## Setup Instructions
### 1. Install Dependencies
Ensure you have Python 3.x installed, then install the required libraries:
```bash
pip install -r requirements.txt
```
Alternatively, install dependencies manually:
```bash
pip install pandas numpy scikit-learn nltk joblib beautifulsoup4 requests
```

### 2. Running the Notebook
Run the provided Jupyter Notebook `code.ipynb` in order:

1. **Data Scraping**: Automatically collects Greeklish and English text.
2. **Preprocessing**: Cleans text and splits paragraphs into sentences.
3. **Model Training**: Trains an SVM classifier.
4. **Evaluation**: Computes accuracy, precision, recall, and F1-score.

#### **Running the Notebook**
Launch Jupyter Notebook:
```bash
jupyter notebook greeklish_scraping.ipynb
```

## Testing the Classifier
To classify a new sentence, run the **inference cell** at the end of the notebook with:
```python
predict_text("ti kaneis")
```
Expected Output:
```
Prediction: Greeklish
```

## Notes
- The model uses **TF-IDF with character n-grams**.
- The SVM classifier is trained using an **RBF kernel**.
- All datasets and models are stored in `/mnt/data/` for easy access.

For further details, refer to the **Documentation PDF**.


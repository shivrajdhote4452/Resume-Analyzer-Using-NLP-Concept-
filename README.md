
# Resume Analyzer Using NLP

An AI-powered **Resume Analyzer** that uses Natural Language Processing (NLP) and Machine Learning to automatically screen resumes, extract key information, and match candidate profiles with relevant job roles.[web:27][web:22]

---

## 🚀 Features

- Upload resume files (PDF/DOCX/TXT) through a simple web interface.[web:22][web:25]  
- Clean and preprocess resume text (lowercasing, stopword removal, lemmatization, etc.).[web:22][web:27]  
- Extract important entities like skills, experience, education, and contact details using NLP techniques.[web:21][web:25]  
- Convert text to numerical features using TF‑IDF or similar vectorization methods.[web:22][web:27]  
- Train and use a machine learning model to classify resumes into job categories or score their relevance to a job description.[web:22][web:26][web:27]  
- Display predictions, similarity/relevance scores, and basic analytics for recruiters or students improving their resumes.[web:24][web:28]  

---

## 🧠 Tech Stack

- Python  
- NLP libraries (NLTK / spaCy / scikit‑learn) for preprocessing, vectorization, and modeling.[web:21][web:22][web:27]  
- Streamlit or Flask for the web interface.[web:22][web:25]  
- Additional libraries for PDF/DOCX parsing (e.g., PyPDF2, pdfplumber, python-docx).[web:21][web:22]  

---

## 📂 Project Structure

```bash
Resume-Analyzer-Using-NLP-Concept/
│
├── app.py                # Main web app script (Streamlit/Flask)
├── model/
│   ├── vectorizer.pkl    # Saved TF-IDF or embedding vectorizer
│   └── model.pkl         # Trained ML classification / ranking model
├── data/
│   └── resumes/          # Sample resumes or dataset
├── notebooks/
│   └── eda_and_training.ipynb  # EDA, preprocessing, model training
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation
```

(Adjust file names/folders to match your actual project.)

---

## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/Resume-Analyzer-Using-NLP-Concept.git
cd Resume-Analyzer-Using-NLP-Concept
```

2. Create and activate a virtual environment (recommended):

```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

3. Install the dependencies:

```bash
pip install -r requirements.txt
```

4. (Optional) Download any additional NLP models (e.g., spaCy language model):

```bash
python -m spacy download en_core_web_sm
```

---

## ▶️ Usage

1. Train or load the model:

- If a trained model is provided (`model/model.pkl` and `model/vectorizer.pkl`), the app will load them directly.[web:22]  
- Otherwise, open `notebooks/eda_and_training.ipynb`, run all cells to train the model, and save the artifacts into the `model/` folder.[web:22][web:27]

2. Run the web application:

```bash
streamlit run app.py
```

(or `python app.py` if you are using Flask.)

3. Open the local URL shown in the terminal, upload a resume, and view:

- Extracted entities and cleaned text  
- Predicted job category / role  
- Relevance or matching score based on a job description (if enabled)  

---

## 📊 How It Works (Pipeline)

1. **Upload**: User uploads a resume file via the UI.[web:22][web:25]  
2. **Parsing**: The file is converted to raw text using PDF/DOCX parsers.[web:21][web:22]  
3. **Preprocessing**: Text cleaning, tokenization, stopword removal, and lemmatization.[web:22][web:27]  
4. **Feature Extraction**: Text is transformed into vectors using TF‑IDF or embeddings.[web:22][web:27]  
5. **Model Inference**: A trained classifier or ranking model predicts job category or similarity to a job description.[web:22][web:26][web:27]  
6. **Output**: The app displays predictions, scores, and insights to help in screening or resume improvement.[web:24][web:28]

---

## 📌 Use Cases

- HR teams automating initial resume screening and shortlisting.[web:24][web:27]  
- Students and job seekers checking how well their resumes align with specific 

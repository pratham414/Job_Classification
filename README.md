**💻 How to Use the Application**

**File Upload:** Use the "Choose a Resume File" button to select and upload your resume in .pdf or .txt format.

**Content Review:** Once uploaded, your resume text will display in a preview area for verification.

**Processing:** Press the "Analyze Resume" button to initiate analysis. A loading indicator will show while the system processes your text using DistilBERT technology and runs it through the classification algorithm.

**Results Display:** The system will present:
- Three recommended job categories ranked by confidence level, shown with visual confidence metrics
- Identified technical skills found throughout your resume

**🗓 Development Timeline Overview**

The project followed a structured four-week development approach:

| Timeframe | Primary Focus | Key Technologies |
|-----------|---------------|------------------|
| Week 1 | Data Processing & Foundation | NLTK, Spacy, TF-IDF |
| Week 2 | Initial Model Development & Testing | Scikit-learn (Naive Bayes, SVM, Logistic Regression) |
| Week 3 | Advanced Model Implementation | DistilBERT (Contextual Embeddings, GPU optimization) |
| Week 4 | Production Deployment & Demo | Streamlit, Joblib (Model Persistence) |

**🧠 Technical Architecture**

The classification system operates through a dual-stage approach:

**Embedding Generation (DistilBERT):** Resume content undergoes tokenization and processing through a pre-trained DistilBERT model. Token outputs are consolidated into a comprehensive vector representation that encodes the semantic context and meaning of the complete resume.

**Category Prediction (Logistic Regression):** A trained Logistic Regression classifier processes these semantic embeddings to determine job category predictions. This hybrid approach delivers strong accuracy while maintaining robust generalization performance.

**🔮 Planned Improvements**

**Advanced BERT Integration:** Move beyond using BERT as a feature extractor to fine-tuning the entire BERT architecture specifically for classification tasks, potentially boosting prediction accuracy.

**Enhanced Skill Detection:** Replace the current keyword-based approach with sophisticated Named Entity Recognition models (such as advanced Spacy implementations) for more precise and adaptable skill identification.

**Interactive Learning System:** Develop a feedback mechanism with database integration to capture user validation of predictions, enabling continuous model improvement through periodic retraining cycles.

**Cloud Infrastructure:** Transition from local Streamlit deployment to cloud-based hosting (AWS EC2 or Streamlit Cloud) to enable broader public access and improved scalability.

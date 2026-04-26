# AIProject_NLP-CLY
AI Project Part 5 Basic Natural Language Processing with Unsupervised Learning with 20 Newsgroups dataset

## **NLP Clustering on the 20 Newsgroups Dataset**

This project applies foundational Natural Language Processing (NLP) techniques to explore structure within the **20 Newsgroups** dataset using **unsupervised learning**.

### **Project Overview**
- Load and preprocess ~18k documents across 20 categories  
- Convert text into numerical features using:
  - Bag of Words (BoW)
  - TF–IDF
  - Optional: GloVe word embeddings  
- Apply clustering algorithms (K‑Means, optional hierarchical)
- Evaluate cluster quality (silhouette score)
- Visualize clusters using PCA
- Predict cluster assignments for new, unseen documents

### **Key Steps**
1. **Preprocessing**  
   Lowercasing, punctuation removal, whitespace normalization, stopword removal.

2. **Feature Extraction**  
   - `CountVectorizer` (BoW)  
   - `TfidfVectorizer` (TF–IDF, 5000 features)  
   - Optional averaged GloVe embeddings (50‑dim)

3. **Clustering**  
   - K‑Means with `k=20`  
   - Top terms extracted per cluster for interpretation

4. **Evaluation**  
   - Silhouette score  
   - Qualitative inspection of cluster themes  
   - PCA 2‑D visualization

5. **Prediction**  
   - Assign clusters to new text inputs using the trained TF–IDF + K‑Means model

### **Results Summary**
- Clusters formed around clear themes (e.g., politics, sports, religion, motorcycles, graphics formats, hardware).  
- TF–IDF produced the most interpretable clusters.  
- New document predictions aligned with expected topics.

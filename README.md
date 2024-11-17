#### **Project Title**  
**Exploring Social Media Reactions to Disasters Using Text Mining and Sentiment Analysis**

---

#### **Project Description**  
Natural disasters and other crises often generate significant social media activity, where people express their thoughts, emotions, and concerns. This project leverages data mining, natural language processing (NLP), and sentiment analysis techniques to explore public reactions to such events.

The project aims to analyze these reactions by:
1. Gathering diverse data from platforms like **Twitter** and **YouTube**.
2. Preprocessing and cleaning the text data for better analysis.
3. Applying sentiment analysis to understand emotional tones.
4. Creating meaningful visualizations for insights.
5. Clustering data to identify thematic patterns.

This repository provides a detailed guide for replicating the analysis and customizing it for other datasets.

---

#### **Key Objectives**
- Understand how people react to disasters on social media.  
- Analyze sentiment (positive, neutral, negative) and emotions (fear, anger, joy, etc.) in user-generated content.  
- Extract key patterns, themes, and word relationships through clustering and co-occurrence analysis.  
- Provide actionable insights for organizations involved in disaster response and public communication.  

---

#### **Features**
- **Data Collection**:  
  - **APIs**: Collected tweets and articles using APIs like Guardian News and World News.  
  - **Web Scraping**: Gathered data from publicly available datasets on Kaggle.  
  - **YouTube Comments**: Extracted comments from disaster-related videos using YouTube’s Data API.

- **Data Cleaning**:  
  - Removed duplicates, missing values, and irrelevant text.  
  - Standardized text through tokenization, lemmatization, and normalization.  
  - Handled outliers and scaled numerical features where applicable.

- **Text Analysis**:  
  - Used NLP tools for preprocessing, including `NLTK`, `SpaCy`, and `TextBlob`.  
  - Sentiment scoring to classify comments as positive, negative, or neutral.  
  - Emotion detection using libraries like NRCLex to identify fear, anger, joy, etc.  

- **Clustering**:  
  - Reduced dimensions of TF-IDF features using TruncatedSVD.  
  - Clustered data using K-Means and visualized results with scatter plots.

- **Visualization**:  
  - Created detailed and interactive plots, including:
    - Word clouds
    - Sentiment histograms and pie charts
    - QQ plots
    - Co-occurrence heatmaps
    - Scatter plots and silhouette plots for clustering  
  - Provided insights for each visualization to contextualize findings.

---

#### **Technologies Used**
- **Languages**: Python  
- **Libraries**:  
  - **Data Handling**: `Pandas`, `NumPy`  
  - **Text Analysis**: `NLTK`, `SpaCy`, `TextBlob`, `VADER`, `NRCLex`  
  - **Visualization**: `Matplotlib`, `Seaborn`, `WordCloud`, `NetworkX`  
  - **Clustering and Dimensionality Reduction**: `Scikit-learn`, `TruncatedSVD`, `KMeans`  
  - **Frequent Pattern Mining**: `mlxtend`  
  - **APIs**: `requests`, `BeautifulSoup`, `YouTube API`  

---

#### **Data Pipeline**
1. **Data Collection**:  
   - APIs (Guardian News, World News, YouTube) and Kaggle datasets were used to collect data.  
   - Data was saved in structured formats like CSV or Excel for further processing.

2. **Data Preprocessing**:  
   - Handled missing values (mean for numerical, mode for categorical).  
   - Removed duplicates and irrelevant data points.  
   - Preprocessed text using tokenization, lemmatization, and removal of stopwords.

3. **Text Mining**:  
   - Extracted key phrases and performed frequency analysis.  
   - Generated TF-IDF vectors for clustering and thematic analysis.  

4. **Clustering**:  
   - Reduced high-dimensional TF-IDF vectors using TruncatedSVD.  
   - Applied K-Means to identify meaningful groups of data.  

5. **Visualization**:  
   - Visualized results to provide actionable insights using advanced plots like scatter plots, network graphs, and silhouette plots.  

---

#### **Visualizations**
- **Word Cloud**: Displays the most frequent words in the dataset, providing a quick overview of prominent themes.  
- **Histogram**: Shows the distribution of sentiment scores across comments.  
- **Pie Chart**: Highlights the proportions of positive, neutral, and negative sentiments.  
- **Scatter Plot**: Visualizes clustering results in 2D space for reduced TF-IDF features.  
- **Silhouette Plot**: Evaluates the quality of clusters formed through K-Means.  
- **Network Graph**: Represents relationships between frequently co-occurring words.  

---

#### **Repository Structure**
```
/project-directory
├── data/                    # Raw and processed datasets
├── notebooks/               # Jupyter notebooks for analysis
├── visuals/                 # Generated plots and visualizations
├── results/                 # Final cleaned data and insights
├── requirements.txt         # Python dependencies
├── Exploring_Social_Media_Reactions_to_Disasters.ipynb  # Main notebook
└── README.md                # This file
```

---

#### **Getting Started**
1. Clone the repository:  
   ```bash
   git clone https://github.com/<username>/<repository-name>.git
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter notebook:  
   ```bash
   jupyter notebook Exploring_Social_Media_Reactions_to_Disasters.ipynb
   ```
4. Run the cells sequentially to replicate the analysis.

---

#### **Usage**
- Modify the notebook to analyze different datasets by replacing the input data files.  
- Use the scripts for custom text mining and sentiment analysis on other topics.  
- Visualizations are reusable; adapt the plotting code for new data.

---

#### **Future Improvements**
- Incorporate real-time data streams from social media platforms like Twitter or Reddit.  
- Explore advanced sentiment analysis models, such as transformers (e.g., BERT).  
- Develop an interactive dashboard for dynamic exploration of the results.  
- Integrate geospatial analysis to map sentiments to specific disaster-affected regions.

---

#### **Contributing**
Contributions are welcome! To contribute:  
1. Fork the repository.  
2. Create a feature branch:  
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes:  
   ```bash
   git commit -m "Add feature description"
   ```
4. Push to the branch:  
   ```bash
   git push origin feature-name
   ```
5. Submit a pull request for review.

---

#### **License**
This project is licensed under the [MIT License](LICENSE).

---

#### **Contact**
For queries or suggestions, feel free to reach out via email or create an issue in the repository.

Let me know if you need further refinements or additional details!

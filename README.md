<h1>Fake News Detection</h1>

<h2>Overview</h2>
<p>This project focuses on detecting <b>Fake News</b> using Natural Language Processing (NLP) and Machine Learning techniques.
The goal is to classify news articles into <b>Fake</b> or <b>Real</b> categories based on textual content.</p>
<p>The model analyzes patterns in news articles and learns distinguishing features that help identify misleading or fabricated information.</p>

<h2>Objective</h2>
<ul>
  <li>Classify news articles as Fake or Real</li>
  <li>Build a complete NLP pipeline for text classification</li>
  <li>Understand feature extraction using TF-IDF</li>
  <li>Evaluate model performance using standard metrics</li>
</ul>

<h2>Dataset</h2>
<p>The dataset consists of two separate files:</p>
<ul>
  <li><b>Fake.csv</b> → Contains fake news articles</li>
  <li><b>True.csv</b> → Contains real news articles</li>
</ul>
<p>Dataset Link: <br><a href="https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets" target="_blank">https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset</a></p>

<h2>Tech Stack</h2>
<ul>
  <li>Python</li>
  <li>Pandas, NumPy</li>
  <li>Matplotlib</li>
  <li>Scikit-learn</li>
  <li>Natural Language Processing (NLP)</li>
</ul>

<h2>Data Preprocessing</h2>
<p>News text contains noise and inconsistencies, so preprocessing steps were applied:</p>
<ul>
  <li>Converted text to lowercase</li>
  <li>Removed URLs</li>
  <li>Removed special characters and punctuation</li>
  <li>Cleaned text stored in a new column</li>
</ul>
<p>These steps ensure uniformity and improve model performance.</p>

<h2>Exploratory Data Analysis (EDA)</h2>
<p>Initial analysis and visualizations were performed to understand the dataset:</p>
<ul>
  <li>Distribution of Fake vs Real news</li>
  <li>Text length distribution</li>
  <li>Inspection of cleaned vs original text</li>
</ul>
<p>This helped identify patterns and validate data quality before training.</p>

<h2>Feature Engineering</h2>
<h3>TF-IDF Vectorization</h3>
<p>Text data was converted into numerical form using TF-IDF:</p>
<ul>
  <li>Transforms text into feature vectors</li>
  <li>Assigns importance to words based on frequency</li>
  <li>Reduces influence of common but less meaningful words</li>
</ul>
<p>This enables the machine learning model to process textual data effectively.</p>

<h2>Model Building</h2>
<h3>Algorithm Used: Logistic Regression</h3>
<ul>
  <li>Supervised learning algorithm for binary classification</li>
  <li>Efficient for large datasets</li>
  <li>Handles high-dimensnal sparse data well</li>
</ul>
<p>
The model was trained using TF-IDF features extracted from cleaned text.</p>

<h2>Model Evaluation</h2>
<p>The model performance was evaluated using:</p>
<ul>
  <li><b>Accuracy Score</b> → Measures overall correctness</li>
  <li><b>Confusion Matrix</b> → Shows prediction breakdown</li>
  <li><b>Classification Report</b>:
    <ul>
      <li>Precision</li>
      <li>Recall</li>io
      <li>F1-score</li>
    </ul>
  </li>
</ul>
<p>These metrics provide a detailed understanding of model performance.</p>

<h2>Visualizations</h2>
<h3>Fake vs Real Distribution</h3>
<p>Shows the balance between fake and real news samples.</p>
<img src="https://github.com/IshitaSinha2002/Fake-News-Detector/blob/main/Confusion%20Matrix.png" width: 500px; height: 400px; object-fit: cover;>
<h3>Confusion Matrix</h3>
<p>Displays actual vs predicted classifications.</p>
<img src="https://github.com/IshitaSinha2002/Fake-News-Detector/blob/main/Fake%20vs%20Real%20Dist.png" width: 500px; height: 400px; object-fit: cover;>
<h3>Text Length Distribution</h3>
<p>Shows variation in length of news articles.</p>
<img src="https://github.com/IshitaSinha2002/Fake-News-Detector/blob/main/News%20Len%20Dist.png" width: 500px; height: 400px; object-fit: cover;>
Both datasets include fields such as title and full news text, which are used for classification.</p>

<h2>Key Insights</h2>
<ul>
  <li>The dataset provides clear separation between fake and real news</li>
  <li>TF-IDF effectively captures important textual patterns</li>
  <li>Logistic Regression performs well for classification tasks</li>
  <li>Certain words strongly influence fake vs real predictions</li>
</ul>

<h2>Prediction System</h2>
<p>A prediction system was implemented to classify new news content as fake or real.</p>
<p>The process includes:</p>
<ul>
  <li>Cleaning the input text using preprocessing steps</li>
  <li>Transforming the text using the trained TF-IDF vectorizer</li>
  <li>Passing the data into the trained model</li>
  <li>Returning the predicted label (Fake or Real)</li>
</ul>

<h3>Sample Input & Output</h3>
<p>Input:  This shocking secret cure for cancer has been hidden by doctors for years!<br>
Output: Fake News</p>

<h2>Conclusion</h2>
<p>This project demonstrates how NLP and machine learning can be used to detect misinformation in textual data.
It highlights the complete workflow from preprocessing to model evaluation and prediction.</p>

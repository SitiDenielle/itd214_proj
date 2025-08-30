Project Background
Overview: This project focuses on analyzing Sephora customer product reviews to understand insights on product sentiment and customer satisfaction. This analysis aims to uncover key drivers of positive and negative reviews.

Business Objectives:
Predict sentiments derive from positive/negative reviews. Identify products with consistent feedbacks and recommend improvements to the products. 
Enable data-driven decisions for product improvements, brand reputation, and customer engagement.
Provide actionable insights that align with Sephora’s goal of continuous improvement and faster reaction to negative reviews.

Problem Statements:
Large volumes of unstructured text reviews are difficult to interpret manually.
Customers express pain points (e.g., formula, residues, packaging) that need systematic extraction.
Sephora requires a real-time monitoring framework to continuously monitor product sentiment.

Work Accomplished
Data Preparation:
Collected product review dataset including stars (numeric rating) and labels (sentiment classes).
Cleaned text by removing stopwords, product names, and redundant phrases.
Balanced dataset to avoid class bias.

Models:
Logistic Regression with TF-IDF/SMOTE.
DistilBERTm Used pre-trained embeddings for improved contextual understanding.

Evaluation:
Compared models using accuracy and weighted F1-score.
DistilBERT achieved the highest performance (Accuracy ~98%, F1 ~99%).
Proceeded with LR for full pipeline due to speed and stability. LR do still provide good accuracy. 

Recommendation and Analysis
Product Improvement: Address negative sentiment themes like formula issues, irritation, packaging flaws.
Brand Reputation & Monitoring: Some products experience sudden spikes in negative sentiment. Repetitive negative reviews from the same brand.

Monitoring Framework: Extend project to a real-time sentiment dashboard to detect spikes in negativity.
Business Impact: Improved satisfaction, reduced returns, stronger product positioning, better loyalty.

AI Ethics

Privacy: Customer reviews are anonymized, but care must be taken not to expose personally identifiable information.
Fairness: Models must avoid bias against certain product categories or customer groups.
Accuracy: Sentiment models can misinterpret sarcasm or context; continuous validation is needed.
Accountability: Sephora must ensure decisions are not solely based on AI outputs.
Transparency: Clearly communicate to stakeholders how sentiment insights are derived from reviews.

Source Codes and Datasets
All source codes (data preparation, modeling, evaluation) are uploaded to GitHub repository.
Final datasets used for modeling (cleaned train/test sets) are included for reproducibility.

Repository includes:
notebooks
data– final cleaned datasets
results– model outputs and evaluation metrics

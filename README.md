# Pharmacy-review-sentiment-analysis
Project Summary: Pharmacy Review Sentiment Analysis
This project performs sentiment analysis on pharmacy reviews to understand customer feedback across various aspects. The key steps involved are:

**Data Loading:** The process begins by loading the pharmacy review data from an Excel file into a pandas DataFrame.

**Text Cleaning:** The raw review text is cleaned and preprocessed to remove noise such as URLs, email addresses, and special characters, ensuring the text is suitable for analysis.

**Sentiment Model Loading:** A pre-trained sentiment analysis model (specifically, distilbert-base-uncased-finetuned-sst-2-english) is loaded using the transformers library. This model is capable of classifying text into positive or negative sentiment.

**Aspect Detection and Sentiment Analysis:** Each cleaned review is analyzed to identify mentions of specific aspects (e.g., Customer Care, Delivery, Price) based on predefined keywords. For each detected aspect, the sentiment of the relevant parts of the review is determined using the loaded sentiment model.

**Results Compilation:** The analysis results, including detected keywords, sentiment labels (Positive/Negative), sentiment vectors (1 for positive, -1 for negative), and confidence scores, are compiled into a structured format.

**Final DataFrame Creation:** A comprehensive pandas DataFrame is created, combining the original reviews with the detailed sentiment analysis results for each aspect.

**Results Export:** The final DataFrame containing all the analysis results is exported to an Excel file for further examination and reporting.

**Summary Statistics Generation:** A summary report is generated, providing an overview of the sentiment distribution (positive vs. negative) for each analyzed aspect across all the reviews.
This process provides a structured approach to understanding customer sentiment from reviews, highlighting areas of strength and weakness based on the feedback.

